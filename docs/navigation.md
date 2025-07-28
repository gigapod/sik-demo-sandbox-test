---
layout: doc
title: Navigation Configuration Guide
description: Explanation of the navigation.yml settings for the Sandbox Jekyll theme
toc: true
---

<section id="snippet-1" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Navigation Configuration</h2>

  <section id="snippet-1-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Main Navigation</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">
          The <code>main</code> section defines the primary navigation menu, supporting dropdowns, mega menus, and direct links.
        </p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-1">View example's code</a>
      </div>
      <div id="collapse-1-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>main:
  - title: Demos
    type: mega-menu-img
    items:
      - title: Demo1
        url: /demo1/
        image: /assets/img/demos/mi1.webp
        image2x: /assets/img/demos/mi1@2x.webp
      - title: Demo2
        url: /demo2/
        image: /assets/img/demos/mi2.webp
        image2x: /assets/img/demos/mi2@2x.webp
  - title: Pages
    type: dropdown
    items:
      - title: About
        submenu:
          - title: About I
            url: /about/
          - title: About II
            url: /about2/
      - title: Services
        submenu:
          - title: Services I
            url: /services/
          - title: Services II
            url: /services2/
</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-1-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Multi-Column Dropdown (Projects)</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">
          A multi-column dropdown menu, useful for displaying portfolios or projects in an organized structure.
        </p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-2">View example's code</a>
      </div>
      <div id="collapse-1-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>  - title: Projects
    type: dropdown-columns
    items:
      - title: Project Pages
        submenu:
          - title: Projects I
            url: /projects-tiles/
      - title: Single Projects
        submenu:
          - title: Single Project I
            url: /projects/sample-with-slider/
</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-1-3">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Mega Menu with Icons (Blocks)</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">
          A mega menu that displays UI components such as Features, Contact, and About with icons.
        </p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-3">View example's code</a>
      </div>
      <div id="collapse-1-3" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>  - title: Blocks
    type: mega-menu-icon
    items:
      - title: Features
        url: /docs/blocks/features.html
        icon: /assets/img/demos/block8.svg
      - title: Contact
        url: /docs/blocks/contact.html
        icon: /assets/img/demos/block5.svg
</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
  
  <section id="snippet-1-4">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Documentation Navigation Example</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">
          The <code>docs</code> type is used for sidebar navigation in documentation pages.
          It organizes links into sections and subcategories for better accessibility.
        </p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-3-1">View example's code</a>
      </div>
      <div id="collapse-3-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code># Documentation Navigation Example
docs_navigation:
  - title: "Getting Started"
    url: "/docs/getting-started"
    children:
      - title: "Installation"
        url: "/docs/installation"
      - title: "Folder Structure"
        url: "/docs/folder-structure"

  - title: "Customization"
    url: "/docs/customization"
    children:
      - title: "Theme Configuration"
        url: "/docs/theme-config"
      - title: "Styling"
        url: "/docs/styling"

  - title: "Advanced"
    url: "/docs/advanced"
    children:
      - title: "Performance"
        url: "/docs/performance"
      - title: "SEO Optimization"
        url: "/docs/seo"</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-2" class="wrapper pt-16">
  <h2 class="display-5 mb-8">One-Page Navigation</h2>

  <section id="snippet-2-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">One-Page Navigation Links</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">
          One-page navigation allows users to click menu links that scroll smoothly to different sections of a single-page website.
        </p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-1">View example's code</a>
      </div>
      <div id="collapse-2-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>onepage:
  links:
    - text: Home
      url: "#home"
    - text: About
      url: "#about"
    - text: Services
      url: "#services"
    - text: Contact
      url: "#contact"
</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

</section>

<section id="snippet-3" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Navigation Types Quick Reference</h2>
<section id="snippet-3-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Navigation Types Quick Reference</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">
          Below is a quick reference table summarizing the different navigation types supported in <code>navigation.yml</code>.
        </p>
      </div>

      <div class="table-responsive">
        <table class="table table-bordered">
          <thead>
            <tr>
              <th>Navigation Type</th>
              <th>Description</th>
              <th>Example</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td><strong>Documentation Navigation</strong></td>
              <td>Sidebar navigation specifically for documentation pages.</td>
              <td><code>type: docs</code></td>
            </tr>
            <tr>
              <td><strong>Mega Menu (Images)</strong></td>
              <td>Displays large dropdown menus with images.</td>
              <td><code>type: mega-menu-img</code></td>
            </tr>
            <tr>
              <td><strong>Dropdown Menu</strong></td>
              <td>A standard multi-level dropdown navigation.</td>
              <td><code>type: dropdown</code></td>
            </tr>
            <tr>
              <td><strong>Dropdown Columns</strong></td>
              <td>Multi-column dropdown layout for structured navigation.</td>
              <td><code>type: dropdown-columns</code></td>
            </tr>
            <tr>
              <td><strong>Mega Menu (Icons)</strong></td>
              <td>Displays UI blocks in a large dropdown with icons.</td>
              <td><code>type: mega-menu-icon</code></td>
            </tr>
            <tr>
              <td><strong>One-Page Navigation</strong></td>
              <td>Links that scroll smoothly to different sections.</td>
              <td><code>onepage: links</code></td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </section>

</section>

