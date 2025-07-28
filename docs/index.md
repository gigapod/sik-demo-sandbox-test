---
layout: doc
title: Getting Started
description: Complete guide to installing and setting up the Sandbox Jekyll theme
toc: true
---
<section id="snippet-1" class="wrapper pt-16">
<h2 class="display-5 mb-8">Getting Started with Sandbox Theme</h2>

<section id="snippet-1-1">
  <h2 class="mb-5 mt-n15 pt-15 zindex-n">Prerequisites</h2>
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Before installing the theme, ensure you have the following installed:</p>
      <ul> 
        <li>Ruby (version 2.7.0 or higher)</li>
        <li>RubyGems</li>
        <li>GCC and Make</li>
      </ul>
    </div>
  </div>
</section>

<section id="snippet-1-2">
  <h2 class="mb-5 mt-n15 pt-15 zindex-n">Installing Jekyll</h2>
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Run the following command to install Jekyll and Bundler:</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-2">View example's code</a>
    </div>
    <div id="collapse-1-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-bash"><code>gem install jekyll bundler</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="snippet-1-3">
  <h2 class="mb-5 mt-n15 pt-15 zindex-n">Verify Installation</h2>
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">After installation, verify Jekyll is installed correctly:</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-3">View example's code</a>
    </div>
    <div id="collapse-1-3" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-bash"><code>jekyll -v</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="snippet-1-4">
  <h2 class="mb-5 mt-n15 pt-15 zindex-n">Theme Installation</h2>
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Download and extract the theme:</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-4">View example's code</a>
    </div>
    <div id="collapse-1-4" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-bash"><code>Unzip the downloaded file
cd sandbox-jekyll-theme</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="snippet-1-5">
  <h2 class="mb-5 mt-n15 pt-15 zindex-n">Install Dependencies</h2>
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Run the following command to install project dependencies:</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-5">View example's code</a>
    </div>
    <div id="collapse-1-5" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-bash"><code>bundle install</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="snippet-1-6">
  <h2 class="mb-5 mt-n15 pt-15 zindex-n">Start Development Server</h2>
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Use the following command to start the local development server:</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-6">View example's code</a>
    </div>
    <div id="collapse-1-6" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-bash"><code>bundle exec rake serve</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="snippet-1-7">
  <h2 class="mb-5 mt-n15 pt-15 zindex-n">Access Local Site</h2>
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Your site should now be running at:</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-7">View example's code</a>
    </div>
    <div id="collapse-1-7" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-text"><code>http://localhost:4000</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="snippet-1-8">
  <h2 class="mb-5 mt-n15 pt-15 zindex-n">Project Structure</h2>
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">The project directory is structured as follows:</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-8">View example's code</a>
    </div>
    <div id="collapse-1-8" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-text"><code>sandbox-jekyll-theme/
├── _data/          # Site configuration files
├── _includes/      # Reusable components
├── _layouts/       # Page layouts
├── _posts/         # Blog posts
├── _sass/          # Sass partials
├── assets/         # Static files
└── _config.yml     # Main configuration</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="snippet-1-9">
  <h2 class="mb-5 mt-n15 pt-15 zindex-n">Configuration</h2>
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Modify the <code>_config.yml</code> file to configure your site settings:</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-9">View example's code</a>
    </div>
    <div id="collapse-1-9" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-yaml"><code># Site Settings
title: Your Site Title
email: your.email@example.com
description: >-
  Your site description
baseurl: ""
url: ""

# Build settings
markdown: kramdown
permalink: /blog/:title/

# Collections
collections:
  projects:
    output: true
    permalink: /projects/:path/
  authors:
    output: true
    permalink: /authors/:path/</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>
</section>
