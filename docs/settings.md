---
layout: doc
title: Theme Configuration Guide
description: Explanation of the theme.yml settings for the Sandbox Jekyll theme
toc: true
---

<section id="snippet-1" class="wrapper pt-16">
  <h2 class="display-5 mb-8">General Theme Settings</h2>

  <section id="snippet-1-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Site Information</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Basic details about your website, including its name, title, and description.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-1">View example's code</a>
      </div>
      <div id="collapse-1-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code># General Settings
site_name: Sandbox
title: "Sandbox - Modern & Multipurpose Jekyll Theme"
description: >-
  An impressive and flawless site template that includes various UI elements and countless features, 
  attractive ready-made blocks and rich pages, basically everything you need to create a unique and 
  professional website.
favicon: "/assets/img/favicon.webp"</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-1-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">SEO Meta Settings</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">These settings control the social media preview images when sharing your site.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-2">View example's code</a>
      </div>
      <div id="collapse-1-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code># Seo Meta Settings
meta_og_image: "/assets/img/meta-image.webp"  # Image used for OpenGraph (Facebook, LinkedIn)
meta_twitter_image: "/assets/img/meta-image.webp"  # Image used for Twitter cards</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-1-3">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Theme Appearance</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Customize the color scheme, fonts, and icons used throughout the theme.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-1-3">View example's code</a>
      </div>
      <div id="collapse-1-3" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code># Site Wide Theme Color Setting
color_scheme: # Aqua Fuchsia Grape Green Leaf Navy Orange Pink Purple Red Sky Violet Yellow

# Site Wide Theme Font Setting
font_scheme: # dm , space , thicccboi , urbanist

# Site Wide Font Icons Setting (FontAwesome, Unicons, etc.)
font_icons_scheme: # https://unicons.iconscout.com/release/v4.0.8/css/line.css</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

</section>

<section id="snippet-2" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Branding & Contact Information</h2>

  <section id="snippet-2-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Site Logos</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Upload different versions of your logo for various themes (light/dark mode).</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-1">View example's code</a>
      </div>
      <div id="collapse-2-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code># Sitewide Logo
logo_1x: "/assets/img/logo.webp"
logo_2x: "/assets/img/logo@2x.webp"
black_logo_1x: "/assets/img/logo-dark.webp"
black_logo_2x: "/assets/img/logo-dark@2x.webp"
light_logo_1x: "/assets/img/logo-light.webp"
light_logo_2x: "/assets/img/logo-light@2x.webp"</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-2-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Contact Details</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Define your business address, phone number, and email contacts.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-2-2">View example's code</a>
      </div>
      <div id="collapse-2-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code>address: 'Moonshine St. 14/05 Light City, London, United Kingdom'
phone_number: "+00 (123) 456 78 90"
email: "tortoizthemes@gmail.com"</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

</section>

<section id="snippet-3" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Integrations & Features</h2>

  <section id="snippet-3-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Disqus Comments</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">Enable Disqus for blog comments, with optional demo mode.</p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-3-1">View example's code</a>
      </div>
      <div id="collapse-3-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code># Disqus Comments
disqus:
  shortname: your-disqus-shortname
  enabled: false
  demo_mode: true
  demo_message: "💡 Comments are disabled for this demo. Configure Disqus in theme.yml when ready!"</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

</section>

<section id="snippet-4" class="wrapper pt-16">
  <h2 class="display-5 mb-8">Analytics & Maps</h2>

  <section id="snippet-4-1">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Google Analytics</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">
          Google Analytics allows you to track website visitors and monitor user behavior.
          Enable it by setting <code>enable: true</code> and adding your tracking key.
        </p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-4-1">View example's code</a>
      </div>
      <div id="collapse-4-1" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code># Google Analytics
google_analytics:
  enable: false  # Set to 'true' to enable tracking
  key: "UA-664136761-1"  # Your Google Analytics tracking ID</code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="snippet-4-2">
    <h2 class="mb-5 mt-n15 pt-15 zindex-n">Google Maps</h2>
    <div class="card mb-12">
      <div class="card-body">
        <p class="mb-0">
          Embed a Google Map of your location. Replace the iframe URL with your own address.
        </p>
      </div>
      <div class="card-footer position-relative">
        <a class="collapse-link collapsed stretched-link" data-bs-toggle="collapse" href="#collapse-4-2">View example's code</a>
      </div>
      <div id="collapse-4-2" class="card-footer bg-dark p-0 accordion-collapse collapse">
        <div class="code-wrapper">
          <div class="code-wrapper-inner">
<pre class="language-yaml"><code># Google Map
google_map: |
  <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d25387.23478654725!2d-122.06115399490332!3d37.309248660190086!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x808fb4571bd377ab%3A0x394d3fe1a3e178b4!2sCupertino%2C%20CA%2C%20USA!5e0!3m2!1sen!2str!4v1645437305701!5m2!1sen!2str" 
    style="width:100%; height: 100%; border:0" allowfullscreen></iframe></code></pre>
          </div>
        </div>
      </div>
    </div>
  </section>

</section>

