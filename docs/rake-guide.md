---
layout: doc
title: Rake Build System
description: Comprehensive guide to the Rake build system in the Sandbox theme
toc: true
---

<section id="snippet-1" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Understanding Rake</h2>

  <section id="snippet-1-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">What is Rake?</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Rake (Ruby Make) is a build automation tool written in Ruby. In the Sandbox theme, it handles:</p>
        <ul>
          <li>Development server management</li>
          <li>Production builds</li>
          <li>Asset optimization</li>
          <li>Image processing</li>
          <li>Task automation</li>
        </ul>
      </div>
    </div>
  </section>

  <section id="snippet-1-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Prerequisites</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Required software and dependencies:</p>
        <ul>
          <li>Ruby (version 2.7.0 or higher)</li>
          <li>RubyGems</li>
          <li>Bundler gem</li>
          <li>ImageMagick or Vips (for image processing)</li>
        </ul>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-2">View installation commands</a>
      </div>
      <div id="collapse-1-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-bash"><code># Install Ruby dependencies
gem install bundler

# Install ImageMagick (MacOS)
brew install imagemagick

# Install ImageMagick (Ubuntu/Debian)
sudo apt-get install imagemagick

# Install project dependencies
bundle install</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-1-3">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Windows Installation Guide</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Installing ImageMagick on Windows:</p>
        <ol>
          <li>Download the appropriate installer:
            <ul>
              <li>Visit the <a href="https://imagemagick.org/script/download.php#windows" target="_blank">ImageMagick Windows Download Page</a></li>
              <li>Choose the appropriate version (recommended: Q16-HDRI-x64)</li>
              <li>Example filename: <code>ImageMagick-7.1.1-21-Q16-HDRI-x64-dll.exe</code></li>
            </ul>
          </li>
          <li>During installation:
            <ul>
              <li>Check "Add to system PATH"</li>
              <li>Check "Install development headers and libraries for C and C++"</li>
              <li>Check "Install legacy utilities (e.g. convert)"</li>
            </ul>
          </li>
          <li>Verify installation:
            <ul>
              <li>Open Command Prompt</li>
              <li>Run <code>magick -version</code></li>
            </ul>
          </li>
        </ol>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-3">View troubleshooting steps</a>
      </div>
      <div id="collapse-1-3" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-plaintext"><code>Common Windows Issues:

1. "Convert not found" error:
   - Rename "convert.exe" to "imagemagick-convert.exe" in ImageMagick installation directory
   - This prevents conflicts with Windows system convert.exe

2. PATH issues:
   - Open System Properties
   - Click "Environment Variables"
   - Add ImageMagick directory to Path (typically C:\Program Files\ImageMagick-7.x.x-Q16)

3. Ruby gem installation fails:
   - Install Visual Studio Build Tools
   - Run: `ridk install` (select options 1, 2, and 3)
   - Reinstall the gem

4. DLL load failed:
   - Install Visual C++ Redistributable
   - Download from Microsoft's website
   - Install both x86 and x64 versions if unsure</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-1-4">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">System Requirements</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Windows-specific requirements:</p>
        <ul>
          <li>Windows 10 or later (recommended)</li>
          <li>Visual C++ Redistributable 2015-2022</li>
          <li>Visual Studio Build Tools (for gem installation)</li>
          <li>At least 2GB free disk space</li>
          <li>Administrator privileges for installation</li>
        </ul>
      </div>
    </div>
  </section>
</section>

<section id="snippet-2" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Core Functionality</h2>

  <section id="snippet-2-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Development Server</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">The <code>serve</code> task provides a development environment with:</p>
        <ul>
          <li>Live reload capability</li>
          <li>Automatic Sass compilation</li>
          <li>Vendor file processing</li>
          <li>Asset watching</li>
        </ul>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-1">View implementation</a>
      </div>
      <div id="collapse-2-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-ruby"><code>desc "Serve the site"
task :serve => [:prepare] do
  begin
    $logger.info "Starting development server..."
    sh "bundle exec jekyll serve --livereload --livereload-min-delay 5 --trace"
  rescue => e
    $logger.error "Serve error: #{e.message}"
    raise
  end
end</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-2-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Production Build</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">The <code>build</code> task creates production-ready assets:</p>
        <ul>
          <li>Minified CSS and JavaScript</li>
          <li>Optimized images</li>
          <li>Compiled Jekyll site</li>
          <li>Environment-specific configurations</li>
        </ul>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-2">View implementation</a>
      </div>
      <div id="collapse-2-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-ruby"><code>desc "Build the site"
task :build => [:prepare] do
  begin
    $logger.info "Building site for production..."
    sh "JEKYLL_ENV=production bundle exec jekyll build"
  rescue => e
    $logger.error "Build error: #{e.message}"
    raise
  end
end</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-3" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Image Processing</h2>

  <section id="snippet-3-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">WebP Conversion</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Automated image optimization features:</p>
        <ul>
          <li>Batch conversion to WebP format</li>
          <li>Original file preservation options</li>
          <li>Size optimization reporting</li>
          <li>Configurable quality settings</li>
        </ul>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-3-1">View usage</a>
      </div>
      <div id="collapse-3-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-bash"><code># Convert images to WebP
bundle exec rake convert_to_webp

# Optimize and remove originals
bundle exec rake optimize_images[true]

# Remove original files
bundle exec rake remove_originals</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-4" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Best Practices</h2>

  <section id="snippet-4-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Development Workflow</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Recommended development workflow:</p>
        <ol>
          <li>Start development server: <code>bundle exec rake serve</code></li>
          <li>Make changes to source files</li>
          <li>Test in development environment</li>
          <li>Optimize images if needed</li>
          <li>Build for production: <code>bundle exec rake build</code></li>
        </ol>
      </div>
    </div>
  </section>

  <section id="snippet-4-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Performance Tips</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Optimize build performance:</p>
        <ul>
          <li>Use incremental builds during development</li>
          <li>Process images in batches</li>
          <li>Maintain clean asset directories</li>
          <li>Regular cache clearing</li>
        </ul>
      </div>
    </div>
  </section>
</section>

<section id="snippet-5" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Troubleshooting</h2>

  <section id="snippet-5-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Common Issues</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Solutions for frequent problems:</p>
        <ul>
          <li><strong>Missing Dependencies:</strong> Run <code>bundle install</code></li>
          <li><strong>Port Conflicts:</strong> Change port in configuration</li>
          <li><strong>Build Failures:</strong> Check error logs and Jekyll environment</li>
          <li><strong>Image Processing Errors:</strong> Verify ImageMagick installation</li>
        </ul>
      </div>
    </div>
  </section>

  <section id="snippet-5-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Debugging</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Debug Rake tasks:</p>
        <ul>
          <li>Enable verbose mode: <code>rake -v task_name</code></li>
          <li>Check Jekyll logs in <code>_site/build.log</code></li>
          <li>Use <code>--trace</code> flag for detailed stack traces</li>
          <li>Monitor system resources during builds</li>
        </ul>
      </div>
    </div>
  </section>
</section>

<section id="snippet-6" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Advanced Usage</h2>

  <section id="snippet-6-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Custom Tasks</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Create custom Rake tasks in <code>Rakefile</code>:</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-6-1">View example</a>
      </div>
      <div id="collapse-6-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-ruby"><code>desc "Custom task description"
task :custom_task do
  puts "Executing custom task..."
  # Add your custom logic here
end

# Task with dependencies
task :custom_task_with_deps => [:prepare, :build] do
  # This task runs after prepare and build
end</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-7" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Command Reference</h2>

  <section id="snippet-7-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Available Commands</h2>
    <div class="card mb-12">
      <div class="card-body">
        <div class="table-responsive">
          <table class="table table-striped">
            <thead>
              <tr>
                <th>Command</th>
                <th>Description</th>
                <th>Usage</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td><code>serve</code></td>
                <td>Start development server</td>
                <td><code>bundle exec rake serve</code></td>
              </tr>
              <tr>
                <td><code>build</code></td>
                <td>Build for production</td>
                <td><code>bundle exec rake build</code></td>
              </tr>
              <tr>
                <td><code>convert_to_webp</code></td>
                <td>Convert images to WebP</td>
                <td><code>bundle exec rake convert_to_webp</code></td>
              </tr>
              <tr>
                <td><code>optimize_images</code></td>
                <td>Convert and optionally remove originals</td>
                <td><code>bundle exec rake optimize_images[true]</code></td>
              </tr>
              <tr>
                <td><code>prepare</code></td>
                <td>Run preparation tasks</td>
                <td><code>bundle exec rake prepare</code></td>
              </tr>
              <tr>
                <td><code>remove_originals</code></td>
                <td>Remove original images</td>
                <td><code>bundle exec rake remove_originals</code></td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
  </section>
</section>
