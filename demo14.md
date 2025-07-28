---
layout: default
title: Demo 14
permalink: /demo14/
custom_color: violet
custom_font: thicccboi
scroll_top_btn:
  enable: true

# Header
header:
  center_nav: true
  transparent: true
  light: true
  button:
    text: Contact
    url: /contact.html
    class: btn-sm btn-primary rounded-pill
  language_select: true

# Hero Section
hero:
  title: We bring rapid solutions for your business.
  subtitle: We are an award winning branding design agency that strongly believes in the power of creative ideas.
  button:
    label: Learn More
    url: "#"
    class: more hover
  image: /assets/img/photos/about18.jpg
  image2x: /assets/img/photos/about18@2x.jpg

# What We Do Section
what_we_do:
  title: What We Do
  subtitle: We make your spending stress-free for you to have the perfect control.
  services:
    - image: /assets/img/photos/se3.jpg
      image2x: /assets/img/photos/se3@2x.jpg
      title: Package Design
      text: Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus magna, vel scelerisque nisl consectetur et. Maecenas faucibus mollis interdum. Maecenas sed diam eget risus varius.
      features:
        - text: Aenean quam ornare curabitur blandit consectetur.
        - text: Nullam quis risus eget urna mollis ornare aenean leo.
        - text: Etiam porta euismod malesuada mollis nisl ornare sem.
        - text: Vivamus sagittis lacus augue rutrum maecenas.
      button:
        label: More Details
        url: "#"
        class: btn btn-soft-leaf rounded-pill mt-6 mb-0
    - image: /assets/img/photos/se4.jpg
      image2x: /assets/img/photos/se4@2x.jpg
      title: Corporate Design
      text: Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus magna, vel scelerisque nisl consectetur et.
      features:
        - text: Aenean quam ornare curabitur blandit consectetur.
        - text: Nullam quis risus eget urna mollis ornare aenean leo.
        - text: Etiam porta euismod malesuada mollis nisl ornare sem.
        - text: Vivamus sagittis lacus augue rutrum maecenas.
      button:
        label: More Details
        url: "#"
        class: btn btn-soft-leaf rounded-pill mt-6 mb-0
      reverse: true

# Join Community Section
community:
  title: Join Our Community
  subtitle: We are trusted by over 5000+ clients. Join them by using our services and grow your business.
  button:
    label: Join Us
    url: "#"
    class: btn btn-white rounded-pill mb-0 text-nowrap
  background: /assets/img/photos/bg10.jpg

# Projects Section
projects:
  title: Our Projects
  subtitle: Check out some of our awesome projects with creative ideas and great design.
  

# Company Facts Section
company_facts:
  title: Company Facts
  subtitle: We are proud of our projects
  counters:
    - count: 1000+
      text: Completed Projects
    - count: 500+
      text: Happy Clients
    - count: 150+
      text: Awards Won

# Testimonials Section
testimonials:
  

# Strategy Section
strategy:
  title: Company Strategy
  subtitle: Just sit and relax while we take care of your business needs.
  process:
    title: Our Working Process
    image: /assets/img/photos/about20.jpg
    image2x: /assets/img/photos/about20@2x.jpg
    steps:
      - number: 1
        title: Collect Ideas
        text: Nulla vitae elit libero pharetra augue dapibus. Praesent commodo cursus. Sed posuere consectetur.
      - number: 2
        title: Data Analysis
        text: Vivamus sagittis lacus vel augue laoreet. Etiam porta sem malesuada magna est at lobortis nulla auctor.
      - number: 3
        title: Finalize Product
        text: Cras mattis consectetur purus sit amet. Aenean lacinia bibendum nulla sed. Donec ullamcorper metus.
  why_choose:
    title: Why Choose Us?
    text: Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus magna, vel scelerisque nisl consectetur et. Maecenas faucibus mollis interdum. Maecenas sed diam eget risus varius.
    image: /assets/img/photos/about19.jpg
    image2x: /assets/img/photos/about19@2x.jpg
    features:
      - text: Aenean quam ornare curabitur blandit consectetur.
      - text: Nullam quis risus eget urna mollis ornare aenean leo.
      - text: Etiam porta euismod malesuada mollis nisl ornare sem.
      - text: Vivamus sagittis lacus augue rutrum maecenas.
    button:
      label: More Details
      url: "#"
      class: btn btn-soft-primary rounded-pill mt-6 mb-0

# Footer CTA
footer_cta:
  title: Join our community by using our services and grow your business.
  button:
    label: Try It For Free
    url: "#"
---
<div class="content-wrapper">
<header class="wrapper bg-soft-primary">
{% include components/navbar/navbar.html 
    classList="center-nav transparent navbar-light"
    logoAlt="logo-dark"
    otherClassList="w-100 d-flex ms-auto"
    otherLanguageSelect=true
    otherBtn=true
    otherBtnClassList="btn btn-sm btn-primary rounded-pill"
    otherBtnText="Contact"
    otherBtnLink="/contact.html"
%}
</header>
<!-- /header -->

{% include components/sections/demo14/hero.html %}
{% include components/sections/demo14/what-we-do.html %}
{% include components/sections/demo14/community.html %}
{% include components/sections/demo14/projects.html %}
{% include components/sections/demo14/company-facts.html %}
{% include components/sections/demo14/testimonials.html %}
{% include components/sections/demo14/strategy.html %}

</div>
{% include components/footer/footer.html 
  style="default"
  bg_color="bg-navy"
  text_color="text-inverse"
  cta=true
  cta_title="Join our community by using our services and grow your business."
  cta_button_text="Try It For Free"
  cta_button_url="#"
%}
