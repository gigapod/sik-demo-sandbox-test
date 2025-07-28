---
layout: doc
title: Projects Configuration
description: Guide to configuring and managing projects in the Sandbox Jekyll theme
toc: true
---

<section id="snippet-1" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Projects Overview</h2>

  <section id="snippet-1-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Project Structure</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Projects are managed through the <code>_projects</code> collection. Each project requires specific frontmatter configuration.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-1">View example's code</a>
      </div>
      <div id="collapse-1-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>---
layout: project
title: "Project Title"
date: 2024-01-01
category: Design
categories: 
  - Design
  - Development
thumbnail: /assets/img/projects/thumb.webp
hero_image: /assets/img/projects/hero.webp
color: purple
gallery:
  - image: "/assets/img/photos/gallery1.webp"
    title: "Gallery Image 1"
---</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-1-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Collection Configuration</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Configure projects collection in <code>_config.yml</code> with appropriate settings.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-2">View example's code</a>
      </div>
      <div id="collapse-1-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>collections:
  projects:
    output: true
    permalink: /projects/:path/

pagination:
  enabled: true
  collections:
    - name: 'projects'
      per_page: 9
      permalink: '/projects/page:num/'</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-2" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Layout Options</h2>

  <section id="snippet-2-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Tiles Layout</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">The <code>tiles</code> layout creates a uniform grid of project cards.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-1">View example's code</a>
      </div>
      <div id="collapse-2-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>---
layout: projects/tiles
title: Project Gallery
permalink: /projects-tiles/
pagination:
  enabled: true
  collection: projects
  per_page: 9
---</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-2-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Filterable Grid Layout</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">The <code>filterable_grid</code> layout adds category filtering capabilities to project display.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-2">View example's code</a>
      </div>
      <div id="collapse-2-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>---
layout: projects/filterable_grid
title: Project Gallery
filters:
  - Design
  - Development
  - Photography
pagination:
  enabled: true
---</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-3" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Project Components</h2>

  <section id="snippet-3-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Gallery Configuration</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Configure image galleries within project pages using the <code>gallery</code> frontmatter.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-3-1">View example's code</a>
      </div>
      <div id="collapse-3-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>gallery:
  - image: "/assets/img/photos/gallery1.webp"
    title: "Design Process"
  - image: "/assets/img/photos/gallery2.webp"
    title: "Final Result"</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-4" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Usage Guidelines</h2>

  <section id="snippet-4-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Accessing Projects</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Access projects in your templates using the <code>site.projects</code> collection:</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-4-1">View example's code</a>
      </div>
      <div id="collapse-4-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-liquid"><code>{% raw %}{% for project in site.projects %}
  <h2>{{ project.title }}</h2>
  <img src="{{ project.thumbnail }}" alt="{{ project.title }}">
{% endfor %}{% endraw %}</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>