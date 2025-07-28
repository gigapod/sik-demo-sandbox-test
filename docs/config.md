---
layout: doc
title: Configuration Guide
description: Detailed breakdown of the Sandbox Jekyll theme's configuration file
toc: true
---

<section id="snippet-1" class="wrapper pt-16">
  <h2 class="display-5 mb-8">General Site & Build Settings</h2>

  <section id="snippet-1-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Site Settings</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">These settings control the basic site details:</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-1">View example's code</a>
      </div>
      <div id="collapse-1-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code># Site Settings
baseurl: ""
url: ""</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-1-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Build Settings</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Configure Jekyll build options:</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-2">View example's code</a>
      </div>
      <div id="collapse-1-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code># Build settings
markdown: kramdown
permalink: /blog/:title/
sass:
  style: compressed
  sass_dir: _sass
  sourcemap: never</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-1-3">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Plugins</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">These plugins extend Jekyll functionality:</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-3">View example's code</a>
      </div>
      <div id="collapse-1-3" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code># Plugins
plugins:
  - jekyll-feed
  - jekyll-seo-tag
  - jekyll-sitemap
  - jekyll-paginate-v2
  - jekyll-watch
  - jekyll-toc</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-1-4">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">TOC Settings</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Configure Table of Contents settings:</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-4">View example's code</a>
      </div>
      <div id="collapse-1-4" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code># TOC Settings for documentation
toc:
  min_level: 2
  max_level: 3
  ordered: false
  numbered_items: true
  auto_ids: true
  sanitize: false</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-2" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Content & Functionality Settings</h2>

  <section id="snippet-2-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Pagination</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Settings for blog and project pagination:</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-1">View example's code</a>
      </div>
      <div id="collapse-2-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code># Pagination
pagination:
  enabled: true
  collections:
    - name: 'posts'
      per_page: 6
      permalink: '/blog/page:num/'</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-2-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Collections</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Define collections for projects and authors:</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-2">View example's code</a>
      </div>
      <div id="collapse-2-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code># Collections
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

  <section id="snippet-2-3">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">LiveReload</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Settings for automatic page reloading:</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-3">View example's code</a>
      </div>
      <div id="collapse-2-3" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code># LiveReload settings
livereload_max_delay: 5
livereload_min_delay: 2.5</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>
