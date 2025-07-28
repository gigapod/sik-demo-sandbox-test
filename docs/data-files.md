---
layout: doc
title: Data Files Configuration
description: Guide to configuring and managing data files in the _data directory of Sandbox Jekyll theme
toc: true
---

<section id="snippet-1" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Data Files Overview</h2>

  <section id="snippet-1-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Navigation Configuration</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">The <code>navigation.yml</code> file controls the site's navigation structure, supporting multiple menu types including mega menus, dropdowns, and icon menus.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-1">View example's code</a>
      </div>
      <div id="collapse-1-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>main:
  - title: Pages
    type: dropdown
    items:
      - title: Services
        submenu:
          - title: Services I
            url: /services/
          - title: Services II
            url: /services2/

  - title: Blocks
    type: mega-menu-icon
    items:
      - title: About
        url: /docs/blocks/about.html
        icon: /assets/img/demos/block1.svg</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-1-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Theme Settings</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">The <code>theme.yml</code> file contains global theme settings including colors, fonts, logos, and meta information.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-2">View example's code</a>
      </div>
      <div id="collapse-1-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>color_scheme: # Aqua Fuchsia Grape Green Leaf Navy Orange Pink Purple Red Sky Violet Yellow
font_scheme: # dm , space , thicccboi , urbanist
logo_1x: "/assets/img/logo.webp"
logo_2x: "/assets/img/logo@2x.webp"
meta_og_image: "/assets/img/meta-image.webp"</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-2" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Content Configuration</h2>

  <section id="snippet-2-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Footer Configuration</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">The <code>footer.yml</code> file manages footer content including blog-specific elements like popular posts, categories, and tags.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-1">View example's code</a>
      </div>
      <div id="collapse-2-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>blog:
  column_1:
    title: Popular Posts
    posts: []
    default_image: /assets/img/photos/a
  
  column_2:
    tags:
      title: Tags
      items:
        - name: Still Life
          url: /tag/still-life</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-2-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Sidebar Configuration</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">The <code>sidebar.yml</code> defines widgets and components that appear in the blog sidebar.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-2">View example's code</a>
      </div>
      <div id="collapse-2-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>widgets:
  - name: search
    title: "Search"
  - name: popular-posts
    title: "Popular Posts"
    limit: 5
  - name: categories
    title: "Browse Categories"</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-3" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Dynamic Content</h2>

  <section id="snippet-3-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Pricing Plans</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">The <code>pricing_plans.json</code> file manages pricing table data with support for monthly/yearly pricing and feature lists.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-3-1">View example's code</a>
      </div>
      <div id="collapse-3-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-json"><code>{
  "plans": [
    {
      "name": "Basic Plan",
      "svg_icon": "shopping-basket.svg",
      "pricing": {
        "monthly": { "amount": 9, "currency": "$", "duration": "mo" },
        "yearly": { "amount": 99, "currency": "$", "duration": "yr" }
      }
    }
  ]
}</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-4" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Search Configuration</h2>

  <section id="snippet-4-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Search Data</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">The <code>search-data.json</code> template generates searchable content from posts and pages.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-4-1">View example's code</a>
      </div>
      <div id="collapse-4-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-json"><code>[
  {
    "title": "Post Title",
    "content": "Post content...",
    "excerpt": "Post excerpt...",
    "category": "Category",
    "tags": ["tag1", "tag2"],
    "url": "/post-url/",
    "date": "01 Jan 2024",
    "author": "Author Name"
  }
]</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-5" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Usage Guidelines</h2>

  <section id="snippet-5-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Accessing Data Files</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Access data files in your templates using the <code>site.data</code> variable:</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-5-1">View example's code</a>
      </div>
      <div id="collapse-5-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-liquid"><code>{% raw %}{% assign navigation = site.data.navigation %}
{% assign theme_settings = site.data.theme %}
{% assign footer = site.data.footer %}{% endraw %}</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>