---
layout: default
title: Demo 20
permalink: /demo20/
custom_color: purple
custom_font: urbanist
page_frame: true
page_frame_bg: bg-pale-primary
scroll_top_btn:
  enable: true

# Hero Section
hero_video:
  poster: /assets/img/photos/movie2.jpg
  video_src: /assets/media/movie2.mp4
  title: "<span class=\"rotator-zoom\">Rapid Solutions,Innovative Thinking,Top-Notch Support</span>"
  subtitle: We are a digital agency specializing in web design, mobile development and seo optimization.

# What We Do Section
what_we_do:
  title: What We Do?
  subtitle: The service we offer is specifically designed to meet your needs.
  services:
    - image: /assets/img/illustrations/ui4.png
      image2x: /assets/img/illustrations/ui4@2x.png
      title: Web Design
      text: Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus magna risus varius.
      features:
        - Aenean quam ornare curabitur blandit.
        - Nullam quis risus eget urna mollis ornare leo.
        - Etiam porta euismod mollis natoque ornare.
      button:
        label: More Details
        url: "#"
    - image: /assets/img/illustrations/ui1.png
      image2x: /assets/img/illustrations/ui1@2x.png
      title: Mobile Development
      text: Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus magna risus varius.
      features:
        - Aenean quam ornare curabitur blandit.
        - Nullam quis risus eget urna mollis ornare leo.
        - Etiam porta euismod mollis natoque ornare.
      button:
        label: More Details
        url: "#"
      image_right: true
    - image: /assets/img/illustrations/ui5.png
      image2x: /assets/img/illustrations/ui5@2x.png
      title: SEO Optimization
      text: Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus magna risus varius.
      features:
        - Aenean quam ornare curabitur blandit.
        - Nullam quis risus eget urna mollis ornare leo.
        - Etiam porta euismod mollis natoque ornare.
      button:
        label: More Details
        url: "#"

# Video Section
video_section:
  poster: /assets/img/photos/movie.jpg
  video_mp4: /assets/media/movie.mp4
  video_webm: /assets/media/movie.webm
  shapes:
    - shape: pale-pink
      type: hex
      position: "top: 1rem; left: -4.2rem;"
    - shape: pale-primary
      type: circle
      position: "bottom: 2rem; right: -3.5rem;"

# Process Section
process_section:
  title: Our Working Process
  subtitle: Find out everything you need to know about creating a business process model
  steps:
    - icon: bulb
      title: 1. Collect Ideas
      text: Etiam porta malesuada magna mollis euismod consectetur leo elit.
    - icon: compare
      title: 2. Data Analysis
      text: Etiam porta malesuada magna mollis euismod consectetur leo elit.
    - icon: delivery-box
      title: 3. Finalize Product
      text: Etiam porta malesuada magna mollis euismod consectetur leo elit.

# Projects Section
projects_section:
  title: Our Projects
  subtitle: Check out some of our awesome projects with creative ideas and great design.
  button:
    label: Start a Project
    url: "/projects-tiles"

# Clients Section
clients_section:
  title: Our Clients
  subtitle: Trusted by over 300+ clients
  description: We bring solutions to make life easier for our customers.
 

# What Makes Us Different Section
different_section:
  title: What Makes Us Different?
  subtitle: We make spending stress free so you have the perfect control.
  video:
    image: /assets/img/photos/about12.jpg
    image2x: /assets/img/photos/about12@2x.jpg
    video_url: /assets/media/movie.mp4
  features:
    - icon: lamp
      title: Creativity
      text: Curabitur blandit lacus porttitor ridiculus mus.
    - icon: bulb
      title: Innovative Thinking
      text: Curabitur blandit lacus porttitor ridiculus mus.
    - icon: puzzle
      title: Rapid Solutions
      text: Curabitur blandit lacus porttitor ridiculus mus.
    - icon: headphone
      title: Top-Notch Support
      text: Curabitur blandit lacus porttitor ridiculus mus.

# Community Section
community_section:
  title: Join Our Community
  subtitle: We are trusted by over 5000+ clients. Join them now and grow your business.
  counters:
    - count: 1000+
      text: Completed Projects
    - count: 50K+
      text: Happy Customers
    - count: 4x
      text: Revenue Growth
  image: /assets/img/photos/about26.png
  image2x: /assets/img/photos/about26@2x.png
---
 
<div class="page-frame bg-pale-primary content-wrapper">
<header class="wrapper">
{% include components/navbar/navbar.html 
    classList="classic transparent position-absolute navbar-dark"
    logoBoth=true
    logoAlt="logo-dark"
    otherClassList="w-100 d-flex ms-auto"
    otherLanguageSelect=true
    otherInfo=true
%}
</header>
<!-- /header -->

{% include components/sections/demo20/hero-video.html %}
{% include components/sections/demo20/what-we-do.html %}
{% include components/sections/demo20/process-section.html %}
{% include components/sections/demo20/projects-section.html %}
{% include components/sections/demo20/clients-section.html %}
{% include components/sections/demo20/different-section.html %}


</div>
{% include components/footer/footer.html 
  style="default"
  bg_color="bg-dark" 
  text_color="text-inverse"
%}
