---
layout: doc
title: Demo Pages Configuration
description: Complete guide to understanding and customizing demo pages in the Sandbox Jekyll theme
toc: true
---

<section id="snippet-1" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Demo Pages Overview</h2>

  <section id="snippet-1-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Basic Structure</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Demo pages are configured through individual markdown files in the root directory (e.g., <code>demo1.md</code>, <code>demo2.md</code>). Each demo uses specific includes from <code>_includes/components/sections/</code> directories.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-1">View example's code</a>
      </div>
      <div id="collapse-1-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>---
layout: demo14
title: Demo Layout 14
permalink: /demo14/

# Hero Section
hero:
  title: Creative. Smart. Awesome.
  subtitle: We are an award winning digital agency that strongly believes in the power of creative ideas.
  button:
    text: Read More
    url: /about
    
# Projects Section
projects:
  title: Our Projects
  subtitle: Check out some of our awesome projects with creative ideas.
---</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-1-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Include Structure</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Each demo has its own includes folder at <code>_includes/components/sections/demo{number}/</code> containing section-specific templates.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-2">View example's code</a>
      </div>
      <div id="collapse-1-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-liquid"><code>_includes/
  └── components/
      └── sections/
          ├── demo1/
          │   ├── hero.html
          │   ├── about.html
          │   └── projects.html
          ├── demo2/
          │   ├── header.html
          │   └── portfolio.html
          └── demo3/
              ├── services.html
              └── testimonials.html</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-2" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Common Section Types</h2>

  <section id="snippet-2-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Hero Sections</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Hero sections are typically the first visual element and can be configured with various styles and content.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-1">View example's code</a>
      </div>
      <div id="collapse-2-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>hero:
  style: "carousel"  # Options: basic, video, carousel
  title: "Welcome to Sandbox"
  subtitle: "Build better websites with Sandbox"
  background_image: "/assets/img/photos/bg1.jpg"
  buttons:
    - text: "Get Started"
      url: "/contact"
      style: "primary"
    - text: "Learn More"
      url: "/about"
      style: "outline"</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-2-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Project Showcases</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Project sections can be displayed in various formats including grids, carousels, and masonry layouts.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-2">View example's code</a>
      </div>
      <div id="collapse-2-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>projects:
  title: "Latest Projects"
  title_class: "fs-16 text-uppercase text-muted mb-3"
  main_title: "Check out some of our awesome projects"
  project_items:
    - image: "/assets/img/photos/pd1.jpg"
      category: "Development"
      title: "Project Title"
      url: "/single-project.html"</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-3" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Layout Customization</h2>

  <section id="snippet-3-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Color Schemes</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Each demo can use custom color schemes defined in the frontmatter or section configurations.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-3-1">View example's code</a>
      </div>
      <div id="collapse-3-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>colors:
  primary: "purple"
  secondary: "yellow"
  background: "light"
  
sections:
  about:
    background_color: "soft-primary"
    text_color: "primary"
  services:
    background_color: "gray"
    text_color: "dark"</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-4" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Common Components</h2>

  <section id="snippet-4-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Navigation</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Configure navigation styles and menu items for each demo layout.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-4-1">View example's code</a>
      </div>
      <div id="collapse-4-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>navigation:
  style: "transparent"  # Options: solid, transparent, sticky
  color: "light"        # Options: light, dark
  button:
    text: "Contact"
    url: "/contact"
    style: "primary"</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-4-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Footer Styles</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Different footer layouts and content configurations available for each demo.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-4-2">View example's code</a>
      </div>
      <div id="collapse-4-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>footer:
  style: "widget"  # Options: simple, widget, extended
  background: "dark"
  logo: "/assets/img/logo-light.png"
  widgets:
    - title: "About Us"
      content: "Company description here"
    - title: "Contact Info"
      contact_details: true</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-5" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Demo Categories</h2>

  <section id="snippet-5-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Corporate Demos (Demo1-Demo8)</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Corporate demos feature business-focused layouts with sections for services, team members, and company information.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-5-1">View example's code</a>
      </div>
      <div id="collapse-5-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-liquid"><code>{% raw %}{% include components/sections/demo1/services.html %}
{% include components/sections/demo1/team.html %}
{% include components/sections/demo1/solutions.html %}

# Common sections in corporate demos:
- Hero with business messaging
- Service offerings
- Team showcase
- Client testimonials
- Case studies/portfolio
- Contact information{% endraw %}</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-5-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Creative Agency Demos (Demo9-Demo15)</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Agency demos emphasize portfolio work, creative services, and dynamic visual elements.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-5-2">View example's code</a>
      </div>
      <div id="collapse-5-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>portfolio:
  style: "grid"  # Options: grid, masonry, carousel
  items_per_row: 3
  show_filters: true
  categories:
    - Branding
    - Digital
    - Motion
  items:
    - title: "Project Name"
      category: "Branding"
      image: "/assets/img/portfolio/1.jpg"</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-5-3">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Product/App Demos (Demo16-Demo23)</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Product-focused demos showcase features, pricing plans, and app screenshots.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-5-3">View example's code</a>
      </div>
      <div id="collapse-5-3" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>features:
  layout: "grid"  # Options: grid, tabs, accordion
  items:
    - icon: "uil-mobile-android"
      title: "Mobile Ready"
      description: "Responsive design that works on all devices"
      
pricing:
  period_toggle: true  # Enable monthly/yearly toggle
  plans:
    - name: "Basic"
      price: 
        monthly: 19
        yearly: 199
      features:
        - "5 Projects"
        - "100 GB Storage"</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-5-4">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Landing Pages (Demo24-Demo34)</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Conversion-focused landing pages with clear CTAs and marketing elements.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-5-4">View example's code</a>
      </div>
      <div id="collapse-5-4" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>cta:
  style: "fullwidth"  # Options: fullwidth, boxed, split
  background: "primary"
  title: "Ready to get started?"
  button:
    text: "Sign Up Now"
    url: "/signup"
    
testimonials:
  style: "carousel"
  autoplay: true
  items:
    - author: "John Doe"
      company: "Company Name"
      content: "Testimonial text here"</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-6" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Advanced Customization</h2>

  <section id="snippet-6-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Custom Section Creation</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Create new sections by adding HTML templates to your demo's section folder.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-6-1">View example's code</a>
      </div>
      <div id="collapse-6-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-liquid"><code>{% raw %}# File: _includes/components/sections/demo1/custom-section.html

<section class="wrapper bg-light">
  <div class="container py-14 py-md-16">
    <div class="row">
      <div class="col-lg-8">
        <h2>{{ page.custom_section.title }}</h2>
        <p>{{ page.custom_section.content }}</p>
      </div>
    </div>
  </div>
</section>{% endraw %}</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-6-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Component Variations</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Customize existing components with different styles and layouts.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-6-2">View example's code</a>
      </div>
      <div id="collapse-6-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>hero_variations:
  - style: "basic"
    classes: "bg-light"
  - style: "video"
    video_url: "path/to/video.mp4"
  - style: "carousel"
    interval: 5000
  - style: "parallax"
    image: "background.jpg"</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-7" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Best Practices</h2>

  <section id="snippet-7-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Performance Optimization</h2>
    <div class="card mb-12">
      <div class="card-body">
        <ul class="mb-0">
          <li>Use appropriate image sizes and formats</li>
          <li>Minimize custom JavaScript</li>
          <li>Leverage built-in lazy loading</li>
          <li>Utilize CSS utility classes</li>
        </ul>
      </div>
    </div>
  </section>

  <section id="snippet-7-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Responsive Design Guidelines</h2>
    <div class="card mb-12">
      <div class="card-body">
        <ul class="mb-0">
          <li>Use Bootstrap grid system consistently</li>
          <li>Test on multiple device sizes</li>
          <li>Implement mobile-first approach</li>
          <li>Consider touch interfaces</li>
        </ul>
      </div>
    </div>
  </section>
</section>
