---
layout: default
title: Demo 2
permalink: /demo2/
custom_color: 
custom_font: dm
scroll_top_btn:
  enable: true 



# Hero Section
hero:
  title: We bring solutions to make life easier for our customers.
  subtitle: We have considered our solutions to support every stage of your growth.
  buttons:
    - label: Explore Now
      url: "#"
      class: btn-lg btn-primary rounded-pill me-2
    - label: Free Trial
      url: "#"
      class: btn-lg btn-outline-primary rounded-pill
  image: /assets/img/photos/about7.jpg
  image2x: /assets/img/photos/about7@2x.jpg

# Services Section
services:
  title: The service we offer is specifically designed to meet your needs.
  subtitle: What We Do?
  items:
    - icon: uil uil-phone-volume
      title: 24/7 Support
      text: Etiam porta sem malesuada magna mollis euismod. Donec ullamcorper nulla non metus auctor fringilla.
    - icon: uil uil-shield-exclamation
      title: Secure Payments
      text: Etiam porta sem malesuada magna mollis euismod. Donec ullamcorper nulla non metus auctor fringilla.
    - icon: uil uil-laptop-cloud
      title: Daily Updates
      text: Etiam porta sem malesuada magna mollis euismod. Donec ullamcorper nulla non metus auctor fringilla.
    - icon: uil uil-chart-line
      title: Market Research
      text: Etiam porta sem malesuada magna mollis euismod. Donec ullamcorper nulla non metus auctor fringilla.

# How It Works Section
how_it_works:
  title: How It Works?
  subtitle: So here are three working steps why our valued customers choose us.
  steps:
    - number: 1
      title: Collect Ideas
      text: Nulla vitae elit libero pharetra augue dapibus. Praesent commodo cursus.
    - number: 2
      title: Data Analysis
      text: Vivamus sagittis lacus vel augue laoreet. Etiam porta sem malesuada magna.
    - number: 3
      title: Finalize Product
      text: Cras mattis consectetur purus sit amet. Aenean lacinia bibendum nulla sed.
  image: /assets/img/photos/about9.jpg
  image2x: /assets/img/photos/about9@2x.jpg

# Projects Section
projects:
  title: Check out some of our awesome projects with creative ideas and great design.
  subtitle: Latest Projects
  limit: 7  # Number of projects to show

# About Video Section
about_video:
  title: Company that believes in the power of creative strategy.
  subtitle: Who Are We?
  text: Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus magna, vel scelerisque nisl consectetur et.
  points:
    - text: Aenean eu leo quam ornare curabitur blandit tempus.
    - text: Nullam quis risus eget urna mollis ornare donec elit.
    - text: Etiam porta sem malesuada magna mollis euismod.
    - text: Fermentum massa vivamus faucibus amet euismod.
  video_url: /assets/media/movie.mp4
  image: /assets/img/photos/about12.jpg
  image2x: /assets/img/photos/about12@2x.jpg

# Team Section
team:
  title: Save your time and money by choosing our professional team.
  subtitle: Meet the Team
  text: Donec id elit non mi porta gravida at eget metus. Morbi leo risus, porta ac consectetur ac, vestibulum at eros tempus porttitor.
  button_text: See All Members
  button_url: "#"
  # Members will be pulled from _data/team_members.json

# Testimonial Section
testimonial:
  # Data will be pulled from _data/testimonials.json
  image: /assets/img/photos/co2.png
  image2x: /assets/img/photos/co2@2x.png
---
<div class="content-wrapper">
<!-- HEADER -->
{% include components/navbar/navbar.html 
    topInfo=true
    wrapperClass="bg-light"
    classList="center-nav transparent navbar-light"
    otherClassList="w-100 d-flex ms-auto"
    otherLanguageSelect=true
    otherBtn=true
    otherBtnClassList="btn btn-sm btn-primary rounded-pill"
    otherBtnText="Contact"
    otherBtnLink="/contact.html"
%}
<!-- /header -->

{% include components/sections/demo2/hero.html %}
{% include components/sections/demo2/clients.html %}
{% include components/sections/demo2/services.html %}
{% include components/sections/demo2/how-it-works.html %}
{% include components/sections/demo2/projects.html %}
{% include components/sections/demo2/about-video.html %}
{% include components/sections/demo2/team.html %}
{% include components/sections/demo2/testimonial.html %}

{% include components/footer/footer.html 
  style="default" 
  bg_color="bg-light"
  text_color="text-dark"
  widget_title_class="text-dark"
  newsletter=true
%}
</div>
