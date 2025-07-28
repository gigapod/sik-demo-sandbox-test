---
layout: doc
title: Authors Configuration
description: Guide to configuring and managing authors in the Sandbox Jekyll theme
toc: true
---

<section id="snippet-1" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Author Configuration</h2>

  <section id="snippet-1-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Basic Structure</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Create author files in the <code>_authors</code> directory. Each author is defined with frontmatter containing personal information and social links.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-1">View example's code</a>
      </div>
      <div id="collapse-1-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>---
layout: blog/author
name: Tortoiz Themes
position: Design Studio
email: contact@tortoizthemes.com
location: Global
avatar: /assets/img/avatars/u5.webp
bio: Tortoiz Themes is a premium design studio focused on creating beautiful, functional and modern website templates for businesses of all sizes.
slug: tortoiz-themes
---</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-1-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Social Links</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Configure social media links for each author using the <code>social</code> array in the frontmatter.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-2">View example's code</a>
      </div>
      <div id="collapse-1-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>social:
  - icon: twitter
    url: https://twitter.com/tortoizthemes
  - icon: facebook-f
    url: https://facebook.com/tortoizthemes
  - icon: dribbble
    url: https://dribbble.com/tortoizthemes
  - icon: instagram
    url: https://instagram.com/tortoizthemes</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-2" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Author Content</h2>

  <section id="snippet-2-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Biography</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Add the author's biography as markdown content after the frontmatter. This content will be displayed on the author's profile page.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-1">View example's code</a>
      </div>
      <div id="collapse-2-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-markdown"><code>Tortoiz Themes is a leading design studio specializing in premium website templates and UI/UX design solutions. Our team combines creative vision with technical expertise to deliver digital experiences that help businesses stand out online.

We believe in design that serves both aesthetics and functionality, creating templates that are not just visually appealing but also optimized for performance, accessibility, and conversion.</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-2-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Required Fields</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">The following fields are required for each author:</p>
        <ul class="mb-0">
          <li><code>layout</code>: Must be set to <code>blog/author</code></li>
          <li><code>name</code>: Author's full name</li>
          <li><code>slug</code>: URL-friendly version of the name</li>
          <li><code>avatar</code>: Path to author's profile image</li>
          <li><code>bio</code>: Short author biography</li>
        </ul>
      </div>
    </div>
  </section>
</section>

<section id="snippet-3" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Usage Examples</h2>

  <section id="snippet-3-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Linking to Authors</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Reference authors in blog posts using their slug:</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-3-1">View example's code</a>
      </div>
      <div id="collapse-3-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>---
layout: post
title: My Blog Post
author: tortoiz-themes
---</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>