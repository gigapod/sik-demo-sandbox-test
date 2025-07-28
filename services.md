---
layout: default
title: Services
permalink: /services/
custom_color:
custom_font: 
scroll_top_btn:
  enable: true

# Header / Hero Section
hero:
  title: "Our Services"
  subtitle: "We are a creative company that focuses on establishing long-term relationships with customers."
  bg_color: "bg-soft-primary"

# Stats Section
stats:
  image: /assets/img/photos/about5.jpg
  image2x: /assets/img/photos/about5@2x.jpg
  card_bg_image: /assets/img/photos/bg3.jpg
  items:
    - count: 7518
      label: "Completed Projects"
    - count: 3472
      label: "Satisfied Customers"
    - count: 2184
      label: "Expert Employees"
    - count: 4523
      label: "Awards Won"

# What We Do Section
what_we_do:
  title: "What We Do?"
  subtitle: "The full service we are offering is specifically designed to meet your business needs and projects."
  services:
    - icon: "phone-volume"
      title: "24/7 Support"
      text: "Nulla vitae elit libero pharetra augue dapibus."
    - icon: "shield-exclamation"
      title: "Secure Payments"
      text: "Vivamus sagittis lacus augue laoreet vel."
    - icon: "laptop-cloud"
      title: "Daily Updates"
      text: "Cras mattis consectetur purus sit amet."
    - icon: "chart-line"
      title: "Market Research"
      text: "Aenean lacinia bibendum nulla sed consectetur."
  images:
    - src: /assets/img/photos/g1.jpg
      src2x: /assets/img/photos/g1@2x.jpg
      class: "col-md-4 offset-md-2 align-self-end"
    - src: /assets/img/photos/g2.jpg
      src2x: /assets/img/photos/g2@2x.jpg
      class: "col-md-6 align-self-end"
    - src: /assets/img/photos/g3.jpg
      src2x: /assets/img/photos/g3@2x.jpg
      class: "col-md-6 offset-md-1"
    - src: /assets/img/photos/g4.jpg
      src2x: /assets/img/photos/g4@2x.jpg
      class: "col-md-4 align-self-start"

# Process Section
process:
  title: "How We Do It?"
  subtitle: "We make your spending stress-free for you to have the perfect control."
  steps:
    - number: "01"
      title: "Concept"
      text: "Nulla vitae elit libero elit non porta gravida eget metus cras. Aenean eu leo quam. Pellentesque ornare."
      active: false
    - number: "02"
      title: "Prepare"
      text: "Vestibulum id ligula porta felis euismod semper. Sed posuere consectetur est at lobortis."
      active: true
    - number: "03"
      title: "Retouch"
      text: "Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Nulla vitae elit libero."
      active: false
    - number: "04"
      title: "Finalize"
      text: "Integer posuere erat, consectetur adipiscing elit. Fusce dapibus, tellus ac cursus commodo."
      active: false

# Video Section
video:
  bg_image: /assets/img/photos/bg1.jpg
  video_url: "https://www.youtube.com/watch?v=26TbMXXOe0I"
  title: "Find out everything you need to know about creating a business process model."

# Pricing Section
pricing:
  title: "Our Pricing"
  subtitle: "We offer great prices, premium and quality products for your business."
  text: "Enjoy a free 30-day trial and experience the full service. No credit card required!"
  button:
    label: "See All Prices"
    url: "#"
  plans:
    - name: "Premium Plan"
      price_monthly: 19
      price_yearly: 199
      currency: "$"
      features:
        - highlight: true
          text: "<strong>5</strong> Projects"
        - highlight: true
          text: "<strong>100K</strong> API Access"
        - highlight: true
          text: "<strong>200MB</strong> Storage"
        - highlight: true
          text: "Weekly <strong>Reports</strong>"
        - highlight: false
          text: "7/24 <strong>Support</strong>"
      button:
        label: "Choose Plan"
        url: "#"
      popular: false
    - name: "Corporate Plan"
      price_monthly: 49
      price_yearly: 499
      currency: "$"
      features:
        - highlight: true
          text: "<strong>20</strong> Projects"
        - highlight: true
          text: "<strong>300K</strong> API Access"
        - highlight: true
          text: "<strong>500MB</strong> Storage"
        - highlight: true
          text: "Weekly <strong>Reports</strong>"
        - highlight: true
          text: "7/24 <strong>Support</strong>"
      button:
        label: "Choose Plan"
        url: "#"
      popular: true

# Let's Talk Section
lets_talk:
  title: "Let's Talk"
  subtitle: "Let's make something great together. We are trusted by over 5000+ clients. Join them by using our services and grow your business."
  text: "Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Maecenas faucibus mollis interdum. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus."
  button:
    label: "Join Us"
    url: "#"
  counter:
    value: "5000+"
    label: "Satisfied Customers"
  images:
    - src: /assets/img/photos/g5.jpg
      src2x: /assets/img/photos/g5@2x.jpg
    - src: /assets/img/photos/g6.jpg
      src2x: /assets/img/photos/g6@2x.jpg
     
---
<div class="content-wrapper">
<header class="wrapper bg-soft-primary">
{% include components/navbar/navbar.html 
    classList="center-nav transparent navbar-light"
    otherClassList="w-100 d-flex ms-auto"
    otherLanguageSelect=true
    otherBtn=true
    otherBtnClassList="btn btn-sm btn-primary rounded-pill"
    otherBtnText="Contact"
    otherBtnLink="/contact"
%}
</header>
<!-- /header -->

{% include components/sections/services/hero.html %}
{% include components/sections/services/stats.html %}
{% include components/sections/services/what-we-do.html %}
{% include components/sections/services/video.html %}
{% include components/sections/services/pricing.html %}
{% include components/sections/services/lets-talk.html %}

{% include components/footer/footer.html 
  style="default"
  bg_color="bg-dark"
  text_color="text-inverse"
%}
</div>
