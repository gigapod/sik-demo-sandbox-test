---
layout: default
title: Demo 3
permalink: /demo3/
custom_color: aqua
custom_font: thicccboi
scroll_top_btn:
  enable: true 
# Hero Section
hero:
  bg_color: dark
  angled: true
  angled_position: lower-start
  title: "Sandbox focuses on <br /><span class=\"typer text-primary text-nowrap\" data-delay=\"100\" data-words=\"customer satisfaction,business needs,creative ideas\"></span><span class=\"cursor text-primary\" data-owner=\"typer\"></span>"
  subtitle: We carefully consider our solutions to support each and every stage of your growth.
  buttons:
    - label: Get Started
      url: "#"
      class: btn-lg btn-primary rounded
  video_url: /assets/media/movie.mp4
  image: /assets/img/photos/about13.webp
  image2x: /assets/img/photos/about13@2x.webp
# Services Section
services:
  title: The service we offer is specifically designed to meet your needs.
  subtitle: What We Do?
  items:
    - icon: uil uil-phone-volume
      title: 24/7 Support
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus. Cras justo.
      link_text: Learn More
      link_url: "#"
    - icon: uil uil-shield-exclamation
      title: Secure Payments
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus. Cras justo.
      link_text: Learn More
      link_url: "#"
    - icon: uil uil-laptop-cloud
      title: Daily Updates
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus. Cras justo.
      link_text: Learn More
      link_url: "#"
    - icon: uil uil-chart-line
      title: Market Research
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus. Cras justo.
      link_text: Learn More
      link_url: "#"
# How It Works Section
how_it_works:
  title: How It Works?
  subtitle: Here are the 3 working steps on success.
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
  image: /assets/img/photos/about7.webp
  image2x: /assets/img/photos/about7@2x.webp
# Why Choose Us Section
why_us:
  title: Why Choose Us?
  subtitle: A few reasons why our valued customers choose us.
  image: /assets/img/photos/about9.webp
  image2x: /assets/img/photos/about9@2x.webp
  accordion_items:
    - title: Professional Design
      content: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel.
      show: true
    - title: Top-Notch Support
      content: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel.
      show: false
    - title: Header and Slider Options
      content: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel.
      show: false
# Join Community Section
join_us:
  bg_image: /assets/img/photos/bg1.webp
  title: Join Our Community
  subtitle: We are trusted by over 5000+ clients. Join them by using our services and grow your business.
  button_text: Join Us
  button_url: "#"
# Case Studies Section
case_studies:
  title: Check out some of our awesome projects with creative ideas and great design.
  subtitle: Case Studies
  limit: 6
# Company Facts Section
company_facts:
  bg_color: soft-primary
  title: We are proud of our works
  subtitle: Company Facts
  counters:
    - value: 1000+
      label: Completed Projects
    - value: 500+
      label: Happy Clients
    - value: 150+
      label: Awards Won
# Testimonials Section
testimonials:
  image: /assets/img/photos/tm1.webp
# Pricing Section
pricing:
  title: We offer great and premium prices.
  subtitle: Our Pricing
  text: Enjoy a <a href="#" class="hover">free 30-day trial</a> and experience the full service. No credit card required!
  button_text: See All Prices
  button_url: "#"
  plans:
    - title: Premium Plan
      monthly_price: 19
      annual_price: 199
      features:
        - label: "<strong>5</strong> Projects"
          included: true
        - label: "<strong>100K</strong> API Access"
          included: true
        - label: "<strong>200MB</strong> Storage"
          included: true
        - label: "Weekly <strong>Reports</strong>"
          included: true
        - label: "7/24 <strong>Support</strong>"
          included: false
      button_text: Choose Plan
      button_url: "#"
      popular: false
    - title: Corporate Plan
      monthly_price: 49
      annual_price: 499
      features:
        - label: "<strong>20</strong> Projects"
          included: true
        - label: "<strong>300K</strong> API Access"
          included: true
        - label: "<strong>500MB</strong> Storage"
          included: true
        - label: "Weekly <strong>Reports</strong>"
          included: true
        - label: "7/24 <strong>Support</strong>"
          included: true
      button_text: Choose Plan
      button_url: "#"
      popular: true
# Contact Section
contact:
  title: Convinced yet? Let's make something great together.
  subtitle: Get In Touch
  image: /assets/img/photos/about14.webp
  image2x: /assets/img/photos/about14@2x.webp
  address: 
    title: Address
  phone:
    title: Phone
  email:
    title: E-mail
    
---
<div class="content-wrapper">
<!-- HEADER -->
<header class="wrapper bg-dark">
{% include components/navbar/navbar.html 
    wrapperClass="bg-dark"
    classList="center-nav transparent navbar-dark"
    logoBoth=true
    logoAlt="logo-dark"
    otherClassList="w-100 d-flex ms-auto"
    otherSearch=true
    otherBtn=true
    otherBtnClassList="btn btn-sm btn-primary rounded"
    otherBtnText="Contact"
    otherBtnLink="/contact/"
%}
</header>
<!-- /header -->

<!-- HERO SECTION -->
{% include components/sections/demo3/hero.html %}

<!-- SERVICES SECTION -->
{% include components/sections/demo3/services.html %}

<!-- HOW IT WORKS SECTION -->
{% include components/sections/demo3/how-it-works.html %}

<!-- WHY CHOOSE US SECTION -->
{% include components/sections/demo3/why-us.html %}

<!-- JOIN COMMUNITY SECTION -->
{% include components/sections/demo3/join-us.html %}

<!-- CASE STUDIES SECTION -->
{% include components/sections/demo3/case-studies.html %}

<!-- COMPANY FACTS SECTION -->
{% include components/sections/demo3/company-facts.html %}

<!-- TESTIMONIALS SECTION -->
{% include components/sections/demo3/testimonials.html %}

<!-- PRICING SECTION -->
{% include components/sections/demo3/pricing.html %}

<!-- CONTACT SECTION -->
{% include components/sections/demo3/contact.html %}

{% include components/footer/footer.html 
  style="default" 
  bg_color="bg-dark"
  container_padding="pt-17 pt-md-19 pb-13 pb-md-15"
  text_color="text-inverse"
%}
</div>