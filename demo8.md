---
layout: default
title: Demo 8
permalink: /demo8/
custom_color: aqua
custom_font: dm
scroll_top_btn:
  enable: true 

# Hero Section
hero:
  title: Crafting project specific solutions with expertise.
  subtitle: We're a company that focuses on establishing long-term relationships with customers.
  buttons:
    - label: Explore Now
      url: "#"
      class: btn btn-lg btn-primary rounded-pill me-2
    - label: Contact Us
      url: "#"
      class: btn btn-lg btn-outline-primary rounded-pill
  image: /assets/img/photos/co3.webp
  image2x: /assets/img/photos/co3@2x.webp
  happy_clients:
    enable: true
    count: 25000+
    text: Happy Clients

# Clients Section
clients:
  title: Trusted by over 25000+ clients
  subtitle: We bring solutions to make life easier for our customers.

# About Section
about:
  title: Who Are We?
  subtitle: We are a digital and branding company that believes in the power of creative strategy and along with great design.
  text: Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus magna, vel scelerisque nisl consectetur et.
  image: /assets/img/photos/about10.webp
  image2x: /assets/img/photos/about10@2x.webp
  features:
    - icon: /assets/img/icons/lineal/target.svg
      title: Our Mission
      text: Dapibus eu leo quam ornare curabitur blandit tempus.
    - icon: /assets/img/icons/lineal/award-2.svg
      title: Our Values
      text: Aenean lacinia bibendum nulla sed consectetur.

# Services Section
services:
  title: What We Do?
  subtitle: The full service we are offering is specifically designed to meet your business needs and projects.
  image: /assets/img/photos/about11.webp
  image2x: /assets/img/photos/about11@2x.webp
  service_items:
    - icon: /assets/img/icons/lineal/megaphone.svg
      title: Marketing
      text: Nulla vitae elit libero pharetra augue dapibus.
    - icon: /assets/img/icons/lineal/target.svg
      title: Strategy
      text: Vivamus sagittis lacus augue laoreet vel.
    - icon: /assets/img/icons/lineal/settings-3.svg
      title: Development
      text: Cras mattis consectetur purus sit amet.
    - icon: /assets/img/icons/lineal/bar-chart.svg
      title: Data Analysis
      text: Aenean lacinia bibendum nulla sed consectetur.

# Testimonial Section
testimonial:

# Team Section
team:
  title: We are proud of our creative team
  subtitle: Just sit back and relax while we take care of your business needs.
  counters:
    - icon: /assets/img/icons/lineal/check.svg
      count: 7518
      text: Completed Projects
    - icon: /assets/img/icons/lineal/user.svg
      count: 3472
      text: Happy Customers
    - icon: /assets/img/icons/lineal/briefcase-2.svg
      count: 2184
      text: Expert Employees

# Video Section
video:
  title: Sandbox Brings Awesomeness
  subtitle: We have considered our solutions to support every stage of your growth.
  video_url: /assets/media/movie.mp4
  image: /assets/img/photos/about12.webp
  image2x: /assets/img/photos/about12@2x.webp
  skills:
    - title: Marketing
      percentage: 100
    - title: Strategy
      percentage: 80
    - title: Development
      percentage: 85

# Pricing Section
pricing:
  title: We offer great and premium prices.
  subtitle: Enjoy a free 30-day trial and experience the full service. No credit card required!
  button:
    label: See All Prices
    url: "#"
  plans:
    - name: Premium Plan
      monthly_price: 19
      yearly_price: 199
      features:
        - text: <strong>5</strong> Projects
          included: true
        - text: <strong>100K</strong> API Access
          included: true
        - text: <strong>200MB</strong> Storage
          included: true
        - text: Weekly <strong>Reports</strong>
          included: true
        - text: 7/24 <strong>Support</strong>
          included: false
      button:
        label: Choose Plan
        url: "#"
    - name: Corporate Plan
      monthly_price: 49
      yearly_price: 499
      popular: true
      features:
        - text: <strong>20</strong> Projects
          included: true
        - text: <strong>300K</strong> API Access
          included: true
        - text: <strong>500MB</strong> Storage
          included: true
        - text: Weekly <strong>Reports</strong>
          included: true
        - text: 7/24 <strong>Support</strong>
          included: true
      button:
        label: Choose Plan
        url: "#"

# FAQ Section
faq:
  title: Frequently Asked Questions
  subtitle: If you don't see an answer to your question, you can send us an email from our contact form.
  questions:
    - question: How do I get my subscription receipt?
      answer: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus.
      active: false
    - question: Are there any discounts for people in need?
      answer: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus.
      active: false
    - question: Do you offer a free trial edit?
      answer: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus.
      active: false
    - question: How do I reset my Account password?
      answer: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus.
      active: false
---
<div class="content-wrapper">
<header class="wrapper bg-light pt-1">
<!-- HEADER -->
{% include components/navbar/navbar.html 
    topAlert=false
    wrapperClass="bg-soft-primary"
    classList="classic transparent navbar-light"
    logoAlt="logo-dark"
    otherClassList="ms-lg-4"
    otherBtn=true
    otherBtnClassList="btn btn-sm btn-primary rounded-pill"
    otherBtnText="Sign in"
    otherBtnModal="modal-signin"
    
%}
</header>
<!-- /header -->

{% include components/sections/demo8/hero.html %}
{% include components/sections/demo8/clients.html %}
{% include components/sections/demo8/about.html %}
{% include components/sections/demo8/services.html %}
{% include components/sections/demo8/testimonial.html %}
{% include components/sections/demo8/team.html %}
{% include components/sections/demo8/video.html %}
{% include components/sections/demo8/pricing.html %}
{% include components/sections/demo8/faq.html %}

{% include components/footer/footer.html 
  style="widgets" 
  bg_color="bg-light"
%}
</div>