---
layout: doc
title: Blog Posts Configuration
description: Comprehensive guide to creating and customizing blog posts, including layouts, styles, and components
toc: true
---

# Blog Posts Guide

## Post Structure

<section id="snippet-1-1">
  <h2 class="mb-5">Basic Post Structure</h2>
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Every post requires specific frontmatter configuration. Create posts in the <code>_posts</code> directory using the format <code>YYYY-MM-DD-title.md</code>.</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-1">View example's code</a>
    </div>
    <div id="collapse-1-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-yaml"><code>---
layout: post
title: "Your Post Title"
date: 2024-01-01
last_modified: 2024-01-02
author: John Doe
category: Category Name
header_style: standard  # or overlay
header_image: /assets/img/photos/header.webp
featured_image: /assets/img/photos/featured.webp
sidebar_position: right  # or left / false
excerpt: Your post excerpt for SEO and previews
tags:
  - Tag 1
  - Tag 2
comments: true  # or false
likes: 5  # optional
---</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>

## Post Layouts

### 1. Standard Layout

<section id="snippet-2-1">
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Standard layout displays the header at the top of the post with no background image.</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-1">View example's code</a>
    </div>
    <div id="collapse-2-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-yaml"><code>---
layout: post
header_style: standard
sidebar_position: false
---</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>

### 2. Overlay Layout

<section id="snippet-2-2">
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Overlay layout features a full-width header with background image and text overlay.</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-2">View example's code</a>
    </div>
    <div id="collapse-2-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-yaml"><code>---
layout: post
header_style: overlay
header_image: /assets/img/photos/bg.webp
---</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>

### 3. Sidebar Variations

<section id="snippet-2-3">
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Posts can include a sidebar on either side or none at all.</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-3">View example's code</a>
    </div>
    <div id="collapse-2-3" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-yaml"><code># Right Sidebar
sidebar_position: right

# Left Sidebar
sidebar_position: left

# No Sidebar
sidebar_position: false</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>

## Post Components

### 1. Header Components

<section id="snippet-3-1">
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Post headers can be customized using the header include component.</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-3-1">View example's code</a>
    </div>
    <div id="collapse-3-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-liquid"><code>{% raw %}{% include components/header/header-post.html 
  header_style=page.header_style
  background_image=page.header_image
  category=page.category
  title=page.title
  meta_date=page.date
  meta_author=page.author
  meta_comments=page.comments
  meta_likes=page.likes
%}{% endraw %}</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>

### 2. Featured Images

<section id="snippet-3-2">
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Featured images appear below the header and can be configured in the frontmatter.</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-3-2">View example's code</a>
    </div>
    <div id="collapse-3-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-liquid"><code>{% raw %}{% include components/blog/post/featured-image.html 
  image_url=page.featured_image 
  image_alt=page.title 
%}{% endraw %}</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>

### 3. Post Meta Information

<section id="snippet-3-3">
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Meta information includes date, author, comments, and likes.</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-3-3">View example's code</a>
    </div>
    <div id="collapse-3-3" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-yaml"><code>date: 2024-01-01
last_modified: 2024-01-02
author: John Doe
comments: true
likes: 5</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>

## Post Features

### 1. Comments System

<section id="snippet-4-1">
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Enable or disable Disqus comments for individual posts.</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-4-1">View example's code</a>
    </div>
    <div id="collapse-4-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-liquid"><code>{% raw %}{% if site.data.theme.disqus.enabled and page.comments != false %}
  {% include components/blog/disqus-comments.html %}
{% endif %}{% endraw %}</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>

### 2. Post Navigation

<section id="snippet-4-2">
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Navigate between posts using previous/next links.</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-4-2">View example's code</a>
    </div>
    <div id="collapse-4-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-liquid"><code>{% raw %}{% include components/blog/post/post-navigation.html 
  previous_url=page.previous.url 
  next_url=page.next.url 
%}{% endraw %}</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>

### 3. Related Posts

<section id="snippet-4-3">
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Display related posts based on categories and tags.</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-4-3">View example's code</a>
    </div>
    <div id="collapse-4-3" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-liquid"><code>{% raw %}{% include components/blog/related-posts.html %}{% endraw %}</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>

## Sidebar Widgets

### 1. Available Widgets

<section id="snippet-5-1">
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Sidebar can include various widgets configured in <code>_data/sidebar.yml</code>.</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-5-1">View example's code</a>
    </div>
    <div id="collapse-5-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-yaml"><code>widgets:
  - name: search
  - name: categories
  - name: popular-posts
  - name: tags
  - name: archive</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>

## Best Practices

### 1. Image Guidelines

- Use optimized images in WebP format
- Recommended header image dimensions: 1920x1080px
- Featured image dimensions: 800x600px
- Compress images for web performance

### 2. SEO Optimization

- Write descriptive titles
- Include meaningful excerpts
- Use relevant categories and tags
- Optimize image alt text
- Include meta description

### 3. Content Structure

- Use proper heading hierarchy
- Break content into sections
- Include relevant images and media
- Format code blocks properly
- Add internal and external links

## Examples

### 1. Standard Post Example

<section id="snippet-6-1">
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Example of a standard post configuration.</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-6-1">View example's code</a>
    </div>
    <div id="collapse-6-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-yaml"><code>---
layout: post
title: "Standard Post Layout Example"
date: 2024-01-01
author: John Doe
category: Development
header_style: standard
featured_image: /assets/img/photos/post1.webp
sidebar_position: false
excerpt: A comprehensive example of standard post layout
tags: 
  - Tutorial
  - Guide
comments: true
---

## Introduction
Your post content here...</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>

### 2. Overlay Post Example

<section id="snippet-6-2">
  <div class="card mb-12">
    <div class="card-body">
      <p class="mb-0">Example of an overlay post with sidebar.</p>
    </div>
    <div class="card-footer position-relative">
      <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-6-2">View example's code</a>
    </div>
    <div id="collapse-6-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
      <div class="code-wrapper">
        <div class="code-wrapper-inner">
<pre class="language-yaml"><code>---
layout: post
title: "Overlay Post Layout Example"
date: 2024-01-02
author: Jane Smith
category: Design
header_style: overlay
header_image: /assets/img/photos/header1.webp
featured_image: /assets/img/photos/featured1.webp
sidebar_position: right
excerpt: A showcase of overlay post layout with right sidebar
tags: 
  - Design
  - UI/UX
comments: true
likes: 10
---

## Introduction
Your post content here...</code></pre>
        </div>
      </div>
    </div>
  </div>
</section>