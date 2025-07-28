---
layout: default
title: Demo 17
permalink: /demo17/
custom_color: navy
scroll_top_btn:
  enable: true 

# Hero Section
hero:
  subtitle: Hello! This is Sandbox
  title: We bring rapid solutions for your business.
  buttons:
    - label: Explore Now
      url: "#"
      class: btn btn-lg btn-primary rounded-pill me-2
    - label: Contact Us
      url: "#"
      class: btn btn-lg btn-outline-primary rounded-pill
  background_image: /assets/img/photos/bg11.jpg

# Services Section
services:
  title: The service we offer is specifically designed to meet your needs.
  subtitle: What We Do?
  service_items:
    - icon: uil uil-phone-volume
      title: 24/7 Support
      text: Fusce dapibus tellus cursus porta tortor condimentum euismod massa justo vehicula sit amet et risus cras.
      link: "#"
      link_text: Learn More
      color: purple
    - icon: uil uil-shield-exclamation
      title: Secure Payments
      text: Fusce dapibus tellus cursus porta tortor condimentum euismod massa justo vehicula sit amet et risus cras.
      link: "#"
      link_text: Learn More
      color: green
    - icon: uil uil-laptop-cloud
      title: Daily Updates
      text: Fusce dapibus tellus cursus porta tortor condimentum euismod massa justo vehicula sit amet et risus cras.
      link: "#"
      link_text: Learn More
      color: orange

# Strategy Section
strategy:
  title: 3 working steps to organize our business projects.
  subtitle: Our Strategy
  text: Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Etiam porta sem malesuada magna mollis euismod eget. Nullam id dolor id nibh ultricies vehicula ut id elit. Nullam quis risus.
  text2: Nullam id dolor id nibh ultricies vehicula ut id elit. Vestibulum id ligula porta felis euismod semper. Aenean lacinia bibendum consectetur.
  button:
    label: Learn More
    url: "#"
    class: btn btn-primary rounded-pill mb-0
  steps:
    - number: "01"
      title: Collect Ideas
      text: Nulla vitae elit libero pharetra augue dapibus. Fusce dapibus, tellus ac cursus commodo.
      color: purple
    - number: "02"
      title: Data Analysis
      text: Vivamus sagittis lacus vel augue laoreet tortor mauris condimentum fermentum.
      color: green
    - number: "03"
      title: Finalize Product
      text: Cras mattis consectetur purus sit amet massa justo sit amet risus consectetur magna elit.
      color: orange

# Facts Section
facts:
  subtitle: Company Facts
  title: We are proud of our works
  counters:
    - count: 1000+
      text: Completed Projects
    - count: 500+
      text: Happy Clients
    - count: 150+
      text: Awards Won

# Testimonials Section
testimonials:
  image: /assets/img/photos/tm1.jpg
  testimonials_list:
    - text: "Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Vestibulum ligula porta felis euismod semper."
      name: Coriss Ambady
      position: Financial Analyst
    - text: "Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Vestibulum ligula porta felis euismod semper."
      name: Cory Zamora
      position: Marketing Specialist
    - text: "Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Vestibulum ligula porta felis euismod semper."
      name: Nikolas Brooten
      position: Sales Manager

# Case Studies Section
case_studies:
  subtitle: Case Studies
  title: Check out some of our awesome projects with creative ideas and great design.
  projects:
    - image: /assets/img/photos/b4.jpg
      title: Ligula tristique quis risus
      date: 14 Apr 2022
      category: Coding
    - image: /assets/img/photos/b5.jpg
      title: Nullam id dolor elit id nibh
      date: 29 Mar 2022
      category: Workspace
    - image: /assets/img/photos/b6.jpg
      title: Ultricies fusce porta elit
      date: 26 Feb 2022
      category: Meeting
    - image: /assets/img/photos/b7.jpg
      title: Morbi leo risus porta eget
      date: 7 Jan 2022
      category: Business Tips

# Team Section
team:
  subtitle: Our Team
  title: Save your time by choosing our professional team.
  text: Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus magna, vel scelerisque nisl consectetur et.
  image: /assets/img/photos/about24.jpg
  image2x: /assets/img/photos/about24@2x.jpg
  features:
    - text: Aenean eu leo quam ornare curabitur blandit tempus.
    - text: Nullam quis risus eget urna mollis ornare donec elit.
    - text: Etiam porta sem malesuada magna mollis euismod.
    - text: Fermentum massa vivamus faucibus amet euismod.

# Why Choose Us Section
why_choose:
  subtitle: Why Choose Us?
  title: A few reasons why our valued customers choose us.
  image: /assets/img/photos/about25.jpg
  image2x: /assets/img/photos/about25@2x.jpg
  accordions:
    - id: headingOne
      collapse_id: collapseOne
      title: Professional Design
      text: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel.
      show: true
    - id: headingTwo
      collapse_id: collapseTwo
      title: Top-Notch Support
      text: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel.
      show: false
    - id: headingThree
      collapse_id: collapseThree
      title: Header and Slider Options
      text: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel.
      show: false

# Call to Action Section
cta:
  title: We are trusted by over 5000+ clients. Join them now and grow your business.
  button:
    label: Get Started
    url: "#"
    class: btn btn-primary rounded-pill
---
<div class="content-wrapper">
<header class="wrapper bg-gray">
{% include components/navbar/navbar.html 
    classList="fancy navbar-light navbar-bg-light caret-none"
    fancy=true
    logoAlt="logo-dark"
    otherClassList="w-100 d-flex ms-auto"
    otherSocial=true
%}
</header>
<!-- /header -->

{% include components/sections/demo17/hero.html %}
<section class="wrapper bg-gray">
  <div class="container">
   <div class="card shadow-none my-n13 my-md-n15 my-lg-n17">
      <div class="card-body py-12 py-lg-14 px-lg-11 py-xl-16 px-xl-13">
{% include components/sections/demo17/services.html %}
{% include components/sections/demo17/strategy.html %}
{% include components/sections/demo17/facts.html %}
{% include components/sections/demo17/testimonials.html %}
{% include components/sections/demo17/case-studies.html %}
{% include components/sections/demo17/team.html %}
{% include components/sections/demo17/why-choose.html %}
{% include components/sections/demo17/cta.html %}
</div>
</div>
</div>
</section>
</div>
{% include components/footer/footer.html 
  style="three-column"
  container_padding="pt-20 pt-lg-21 pb-7"
  bg_color="bg-dark" 
  text_color="text-inverse"
%}
