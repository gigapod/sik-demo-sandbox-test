---
layout: doc
title: Component Variations
description: Guide to all available navbar, footer, and header variations in the Sandbox theme
toc: true
---

<section id="snippet-1" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Navbar Variations</h2>

  <section id="snippet-1-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Center Nav Variations</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Center-aligned navigation variations with different styles and features.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-1">View example's code</a>
      </div>
      <div id="collapse-1-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-liquid"><code>{% raw %}{% include components/navbar/navbar.html 
    classList="center-nav transparent navbar-light"
    logoBoth=true
    logoAlt="logo-dark"
    otherClassList="w-100 d-flex ms-auto"
    otherSearch=true
    otherBtn=true
    otherBtnClassList="btn btn-sm btn-primary rounded"
    otherBtnText="Contact"
%}{% endraw %}</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-1-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Fancy Navbar Variations</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Enhanced navbar designs with additional styling and features.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-2">View example's code</a>
      </div>
      <div id="collapse-1-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-liquid"><code>{% raw %}{% include components/navbar/navbar-fancy.html 
    wrapperClass=""
    classList="fancy navbar-light navbar-bg-light caret-none"
    centerNav=true
    fancy=true
    logoAlt=true
    otherClassList="w-100 d-flex ms-auto"
    otherSocial=true
%}{% endraw %}</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-2" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Footer Variations</h2>

  <section id="snippet-2-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Default Footer</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Standard four-column footer with newsletter and CTA options.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-1">View example's code</a>
      </div>
      <div id="collapse-2-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-liquid"><code>{% raw %}{% include components/footer/footer.html 
    style="default"
    bg_color="bg-light"
    text_color=""
    newsletter=true
    cta=true
    cta_title="Join our community"
%}{% endraw %}</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-2-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Minimal Footer</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Simplified footer design for landing pages and minimal layouts.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-2">View example's code</a>
      </div>
      <div id="collapse-2-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-liquid"><code>{% raw %}{% include components/footer/footer.html 
    style="minimal"
    bg_color="bg-light"
    text_color=""
%}{% endraw %}</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-3" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Header Variations</h2>

  <section id="snippet-3-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">About Header</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Header design optimized for about and company pages.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-3-1">View example's code</a>
      </div>
      <div id="collapse-3-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-liquid"><code>{% raw %}{% include components/header/header-about.html 
    background_class="bg-soft-primary"
    title="About Us"
    subtitle="A company turning ideas into beautiful things."
    figure_image="/assets/img/photos/bg12.jpg"
%}{% endraw %}</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-3-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Blog Post Header</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Enhanced header design for blog posts with meta information.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-3-2">View example's code</a>
      </div>
      <div id="collapse-3-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-liquid"><code>{% raw %}{% include components/header/header-post.html 
    background_class="image-wrapper bg-image bg-overlay text-white"
    background_image="/assets/img/photos/bg5.jpg"
    category="Teamwork"
    title="Commodo Dolor Bibendum"
    meta_date="5 Jul 2022"
    meta_author="Sandbox"
%}{% endraw %}</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>

<section id="snippet-4" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Configuration Options</h2>

  <section id="snippet-4-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Common Parameters</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Available configuration options for components.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-4-1">View parameters</a>
      </div>
      <div id="collapse-4-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code># Navbar Parameters
classList: "center-nav transparent navbar-light"
logoBoth: true
logoAlt: "logo-dark"
otherClassList: "w-100 d-flex ms-auto"
otherSearch: true
otherBtn: true

# Footer Parameters
style: "default"
bg_color: "bg-light"
text_color: ""
newsletter: true
cta: true

# Header Parameters
background_class: "bg-soft-primary"
title: "Page Title"
subtitle: "Page subtitle"
figure_image: "/path/to/image.jpg"</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>
</section>