---
layout: doc
title: Using Sandbox Without Rake
description: Comprehensive guide to using the Sandbox theme without the Rake build system
toc: true
---

<section id="snippet-1" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Basic Setup</h2>

  <section id="snippet-1-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Direct Jekyll Usage</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">The Sandbox theme can be run directly with Jekyll commands:</p>
        <ul>
          <li>Development server with live reload</li>
          <li>Production builds</li>
          <li>Built-in Sass compilation</li>
          <li>Asset processing</li>
        </ul>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-1">View commands</a>
      </div>
      <div id="collapse-1-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-bash"><code># Start development server
bundle exec jekyll serve --livereload --livereload-min-delay 5

# Build for production
JEKYLL_ENV=production bundle exec jekyll build</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-1-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Prerequisites</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Required software:</p>
        <ul>
          <li>Ruby (version 2.7.0 or higher)</li>
          <li>RubyGems</li>
          <li>Bundler gem</li>
          <li>ImageMagick or Vips (for image processing)</li>
        </ul>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-2">View installation</a>
      </div>
      <div id="collapse-1-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-bash"><code># Install Ruby dependencies
gem install bundler

# Install project dependencies
bundle install</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-2" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Built-in Features</h2>

  <section id="snippet-2-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Sass Processing</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Jekyll includes built-in Sass compilation:</p>
        <ul>
          <li>Automatic processing of Sass files</li>
          <li>Production minification</li>
          <li>Source mapping options</li>
          <li>Custom import paths</li>
        </ul>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-1">View configuration</a>
      </div>
      <div id="collapse-2-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code># _config.yml
sass:
  style: compressed
  sass_dir: _sass
  sourcemap: never</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-3" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Image Processing</h2>

  <section id="snippet-3-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Manual Image Optimization</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Using ImageMagick directly for image processing:</p>
        <ul>
          <li>WebP conversion</li>
          <li>Batch processing</li>
          <li>Image optimization</li>
          <li>Format conversion</li>
        </ul>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-3-1">View commands</a>
      </div>
      <div id="collapse-3-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-bash"><code># Convert single image
magick convert input.jpg -quality 90 output.webp

# Batch convert (PowerShell)
Get-ChildItem -Path "assets/img" -Recurse -Include *.jpg,*.png | 
ForEach-Object { magick convert $_.FullName -quality 90 "$($_.DirectoryName)\$($_.BaseName).webp" }

# Batch convert (Bash/Linux)
find assets/img -type f \( -iname "*.jpg" -o -iname "*.png" \) -exec convert {} -quality 90 {}.webp \;</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-4" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Development Workflow</h2>

  <section id="snippet-4-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Recommended Steps</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Development workflow without Rake:</p>
        <ol>
          <li>Start Jekyll server: <code>bundle exec jekyll serve --livereload</code></li>
          <li>Make changes to source files (Sass compiles automatically)</li>
          <li>Process images manually as needed</li>
          <li>Build for production: <code>JEKYLL_ENV=production bundle exec jekyll build</code></li>
        </ol>
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
          <li><strong>Sass Compilation Errors:</strong> Check <code>_sass</code> directory structure</li>
          <li><strong>Server Start Issues:</strong> Verify port availability</li>
          <li><strong>Build Failures:</strong> Check Jekyll environment settings</li>
          <li><strong>Image Processing:</strong> Confirm ImageMagick installation</li>
        </ul>
      </div>
    </div>
  </section>

  <section id="snippet-5-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Debugging</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Debug Jekyll processes:</p>
        <ul>
          <li>Use verbose mode: <code>jekyll serve --verbose</code></li>
          <li>Check build output in <code>_site</code> directory</li>
          <li>Enable trace mode with <code>--trace</code></li>
          <li>Review Jekyll's error messages</li>
        </ul>
      </div>
    </div>
  </section>
</section>

<section id="snippet-6" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Shell Scripts</h2>

  <section id="snippet-6-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Automation Scripts</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Create shell scripts for common tasks:</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-6-1">View example</a>
      </div>
      <div id="collapse-6-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-bash"><code>#!/bin/bash
# build.sh - Production build script

echo "Building site for production..."
JEKYLL_ENV=production bundle exec jekyll build

echo "Processing images..."
find assets/img -type f \( -iname "*.jpg" -o -iname "*.png" \) -exec convert {} -quality 90 {}.webp \;</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>