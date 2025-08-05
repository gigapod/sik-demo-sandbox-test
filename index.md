---
layout: default
title: SparkFun Inventor's Kit
permalink: /
custom_color: red
custom_font: thicccboi
scroll_top_btn:
  enable: true

# Hero Section
hero:
  image: /assets/img/photos/homepage/sik-robot-collage.png
  background: /assets/img/photos/homepage/sik-hero-background.png
  slider:
    - image: /assets/img/photos/sik-home-slider-1.webp
      image2x: /assets/img/photos/sik-home-slider-1@2x.webp
    - image: /assets/img/photos/sik-home-slider-2.webp
      image2x: /assets/img/photos/sik-home-slider-2@2x.webp
      video: /assets/media/movie.mp4
    - image: /assets/img/photos/sik-home-slider-3.webp
      image2x: /assets/img/photos/sik-home-slider-3@2x.webp
    - image: /assets/img/photos/sik-home-slider-4.webp
      image2x: /assets/img/photos/sik-home-slider-4@2x.webp

# SIK Steps
how_it_works:
  title: Jumping in for the first time?
  subtitle: Beginners start here.
  steps:
    - number: 1
      title: Initially Assembly
      text: Open up your SIK for MicroPython box and get aquainted with all the parts you’ll be using to complete the 5 projects.
    - number: 2
      title: Choose Your Coding Platform
      text: You have two options to dive into the SIK for MicroPython. You can utilize our fully documented Jupiter Notebook (recommended) on any browser or use any MicroPython IDE (Thonny, PieCharm, etc.).
    - number: 3
      title: Dive Into Project 1
      text: Get started by diving into the Jupyter Notebook.
  buttons:
    - label: Launch Notebook
      url: "https://gigapod.dev/jupyter-lite-micropython/lab/index.html"
      class: btn btn-md btn-white rounded-pill me-2
    - label: Follow IDE Guide
      url: "/projects/sfe-test-project/"
      class: btn btn-sm btn-white rounded-pill me-2
  image: /assets/img/photos/homepage/sik-robot-collage.png
    
# Projects Section
portfolio7:
  enable: true
  content:
    subtitle: "Latest Projects"
    subtitle_classes: "fs-16 text-uppercase text-primary mb-3"
    title: "Check out some of our awesome projects with creative ideas and great design."
    title_classes: "display-3 mb-10"
  layout:
    header_column: "col-lg-10 col-xl-9 col-xxl-8 mx-auto text-center"
  swiper:
    margin: 30
    dots: false
    nav: true
    items:
      md: 2
      xs: 1
    classes: "grid-view nav-bottom nav-color mb-14"
  project:
    figure_classes: "rounded mb-7"
    details_classes: "d-flex justify-content-center flex-column"
    title_classes: "post-title h3"
    category_classes: "post-category text-ash"

# Footer CTA
footer_cta:
  title: Start your adventure with the SparkFun Inventor's Kit today!
  button:
    text: Visit SparkFun.com
    url: "https://www.sparkfun.com/sparkfun-inventor-s-kit-v4-1-2.html"
    
  
---
<div class="content-wrapper">
<header class="wrapper bg-soft-primary">
{% include components/navbar/navbar.html 
    topAlert=false
    wrapperClass="bg-soft-primary"
    classList="classic transparent position-absolute navbar-dark"
    logoBoth=true
    logoAlt="logo-dark"
    otherClassList="ms-lg-4"
    otherBtn=true
    otherBtnClassList="btn btn-sm btn-white rounded-pill"
    otherBtnText="Free Trial"
    otherBtnLink="#"
    
%}
</header>
<!-- /header -->

{% include components/sections/demo11/hero.html %}
{% include components/sections/demo2/how-it-works.html %}
{% include components/sections/demo16/projects.html %}

</div>
{% include components/footer/footer.html 
  style="default"
  bg_color="bg-navy"
  text_color="text-inverse"
  cta=true
  cta_title="Start your adventure with the SparkFun Inventor's Kit today!"
  cta_button_text="Purchase at SparkFun.com"
  cta_button_url="https://www.sparkfun.com/sparkfun-inventor-s-kit-v4-1-2.html"
%}
