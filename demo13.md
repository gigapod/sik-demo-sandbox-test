---
layout: default
title: Demo 13
permalink: /demo13/
custom_color: purple
custom_font: thicccboi
scroll_top_btn:
  enable: true

# Hero Section
hero:
  title: We bring rapid solutions for your business
  subtitle: Hello! This is Sandbox
  video_url: /assets/media/movie.mp4
  background: /assets/img/photos/bg2.jpg

# About Section
about:
  image: /assets/img/photos/about5.jpg
  image2x: /assets/img/photos/about5@2x.jpg
  stats_background: /assets/img/photos/bg2.jpg
  stats_items:
    - count: 7518
      text: Completed Projects
    - count: 3472
      text: Satisfied Customers
    - count: 2184
      text: Expert Employees
    - count: 4523
      text: Awards Won

# Services Section
services:
  title: What We Do?
  subtitle: The full service we are offering is specifically designed to meet your business needs and projects.
  service_items:
    - icon: uil uil-phone-volume
      title: 24/7 Support
      text: Nulla vitae elit libero pharetra augue dapibus.
    - icon: uil uil-shield-exclamation
      title: Secure Payments
      text: Vivamus sagittis lacus vel augue laoreet vel.
    - icon: uil uil-laptop-cloud
      title: Daily Updates
      text: Cras mattis consectetur purus sit amet.
    - icon: uil uil-chart-line
      title: Market Research
      text: Aenean lacinia bibendum nulla sed consectetur.

# Process Section
process:
  title: How We Do It?
  subtitle: We make your spending stress-free for you to have the perfect control.
  steps:
    - number: "01"
      title: Concept
      text: Nulla vitae elit libero elit non porta gravida eget metus cras. Aenean eu leo quam. Pellentesque ornare.
      active: false
    - number: "02"
      title: Prepare
      text: Vestibulum id ligula porta felis euismod semper. Sed posuere consectetur est at lobortis.
      active: true
    - number: "03"
      title: Retouch
      text: Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Nulla vitae elit libero.
      active: false
    - number: "04"
      title: Finalize
      text: Integer posuere erat, consectetur adipiscing elit. Fusce dapibus, tellus ac cursus commodo.
      active: false

# Testimonials Section
testimonials:
  title: Happy Customers
  background: /assets/img/photos/bg2.jpg
  

# Portfolio Section
portfolio:
  title: Recent Projects
  subtitle: We love to turn ideas into beautiful things.
  

# Clients Section
clients:
  title: Trusted by over 300+ clients
  subtitle: We bring solutions to make life easier for our customers.
  
# Pricing Section
pricing:
  title: Our Pricing
  subtitle: We offer great prices, premium and quality products for your business.
  trial_text: Enjoy a free 30-day trial and experience the full service. No credit card required!
  button_text: See All Prices
  button_url: "#"
  pricing_plans:
    - title: Premium Plan
      price_monthly: 19
      price_yearly: 199
      yearly_savings: 30
      features:
        - text: <strong>5</strong> Projects
          enabled: true
        - text: <strong>100K</strong> API Access
          enabled: true
        - text: <strong>200MB</strong> Storage
          enabled: true
        - text: Weekly <strong>Reports</strong>
          enabled: true
        - text: 7/24 <strong>Support</strong>
          enabled: false
      button_text: Choose Plan
      button_url: "#"
      popular: false
    - title: Corporate Plan
      price_monthly: 49
      price_yearly: 499
      yearly_savings: 30
      features:
        - text: <strong>20</strong> Projects
          enabled: true
        - text: <strong>300K</strong> API Access
          enabled: true
        - text: <strong>500MB</strong> Storage
          enabled: true
        - text: Weekly <strong>Reports</strong>
          enabled: true
        - text: 7/24 <strong>Support</strong>
          enabled: true
      button_text: Choose Plan
      button_url: "#"
      popular: true

# Let's Talk Section
lets_talk:
  title: Let's Talk
  subtitle: Let's make something great together. We are trusted by over 5000+ clients. Join them by using our services and grow your business.
  text: Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Maecenas faucibus mollis interdum. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus.
  button_text: Join Us
  button_url: "#"
  counter:
    count: 5000+
    text: Satisfied Customers
  images:
    - image: /assets/img/photos/g5.jpg
      image2x: /assets/img/photos/g5@2x.jpg 
    - image: /assets/img/photos/g6.jpg
      image2x: /assets/img/photos/g6@2x.jpg
---
<div class="content-wrapper">
<header class="wrapper bg-soft-primary">
{% include components/navbar/navbar-center-logo.html 
    classList="center-logo transparent position-absolute navbar-dark"
    fancy=false
    logoBoth=true
    logoLight=true
%}
</header>
<!-- /header -->

{% include components/sections/demo13/hero.html %}
{% include components/sections/demo13/about.html %}
{% include components/sections/demo13/services.html %}
{% include components/sections/demo13/testimonials.html %}
{% include components/sections/demo13/portfolio.html %}
{% include components/sections/demo13/clients.html %}
{% include components/sections/demo13/pricing.html %}
{% include components/sections/demo13/letstalk.html %}

</div>
{% include components/footer/footer.html 
  style="default"
  bg_color="bg-dark"
  container_padding="pt-17 pt-md-19 pb-13 pb-md-15"
  text_color="text-inverse"
  cta=false
  
%}
