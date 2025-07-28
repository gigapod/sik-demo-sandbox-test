---
layout: default
title: Services
permalink: /services2/
custom_color:
custom_font: 
scroll_top_btn:
  enable: true

# Header / Hero Section
hero:
  title: "Our Services"
  subtitle: "We are a creative company that focuses on establishing long-term relationships with customers."
  bg_image: "/assets/img/photos/bg1.jpg"
  bg_overlay: true

# What We Do Section
what_we_do:
  title: "What We Do?"
  subtitle: "The service we offer is specifically designed to meet your needs."
  text: "Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Maecenas sed diam eget risus varius blandit sit amet non magna. Maecenas faucibus mollis interdum. Praesent commodo cursus magna, vel scelerisque nisl consectetur et."
  button:
    label: "More Details"
    url: "#"
  cards:
    - icon: "telephone-3"
      color: "yellow"
      title: "24/7 Support"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta."
    - icon: "shield"
      color: "red"
      title: "Secure Payments"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta."
    - icon: "cloud-computing-3"
      color: "leaf"
      title: "Daily Updates"
      text: "Nulla vitae elit libero, a pharetra augue."
    - icon: "analytics"
      color: "primary"
      title: "Market Research"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget."

# Video Section
video:
  poster: "/assets/img/photos/movie.jpg"
  url: "/assets/media/movie.mp4"
  webm_url: "/assets/media/movie.webm"

# Process Section
process:
  title: "Our Process"
  subtitle: "Find out everything you need to know about creating a business process model"
  steps:
    - number: "1"
      icon: "light-bulb"
      color: "primary"
      title: "Concept"
      text: "Nulla vitae elit libero elit non porta gravida eget metus cras."
    - number: "2"
      icon: "settings-3"
      color: "red"
      title: "Prepare"
      text: "Nulla vitae elit libero elit non porta gravida eget metus cras."
    - number: "3"
      icon: "design"
      color: "leaf"
      title: "Retouch"
      text: "Nulla vitae elit libero elit non porta gravida eget metus cras."

# Features Section Configuration
section1:
  image: "/assets/img/illustrations/i8.png"
  image2x: "/assets/img/illustrations/i8@2x.png"
  title: "We bring rapid solutions to make the life of our customers easier."
  progress_items:
    - name: "Marketing"
      value: 100
      color: "blue"
    - name: "Strategy"
      value: 80
      color: "yellow"
    - name: "Development"
      value: 85
      color: "orange"
    - name: "Data Analysis"
      value: 90
      color: "green"

section2:
  image: "/assets/img/illustrations/i7.png"
  image2x: "/assets/img/illustrations/i7@2x.png"
  title: "We make your spending stress-free for you to have the perfect control."
  description: "Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus magna, vel scelerisque nisl consectetur et."
  features:
    - "Aenean quam ornare. Curabitur blandit."
    - "Nullam quis risus eget urna mollis ornare."
    - "Etiam porta euismod malesuada mollis."
    - "Vivamus sagittis lacus vel augue rutrum."

# Pricing Section
pricing:
  title: "Our Pricing"
  subtitle: "We offer great prices, premium products and quality service for your business."
  plans:
    - name: "Basic Plan"
      icon: "shopping-basket"
      price_monthly: 9
      price_yearly: 99
      currency: "$"
      features:
        - highlight: true
          text: "<strong>1</strong> Project"
        - highlight: true
          text: "<strong>100K</strong> API Access"
        - highlight: true
          text: "<strong>100MB</strong> Storage"
        - highlight: false
          text: "Weekly <strong>Reports</strong>"
        - highlight: false
          text: "7/24 <strong>Support</strong>"
      button:
        label: "Choose Plan"
        url: "#"
      popular: false
    - name: "Premium Plan"
      icon: "home"
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
      popular: true
    - name: "Corporate Plan"
      icon: "briefcase-2"
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
      popular: false

# Community Section
community:
  title: "Join Our Community"
  subtitle: "We are trusted by over 5000+ clients. Join them now and grow your business."
  bg_image: "/assets/img/map.png"
  counters:
    - count: 7518
      label: "Completed Projects"
    - count: 5472
      label: "Satisfied Customers"
    - count: 2184
      label: "Expert Employees"
---
<div class="content-wrapper">
<header class="wrapper bg-soft-primary">
{% include components/navbar/navbar.html 
    classList="center-nav transparent position-absolute navbar-dark"
    logoBoth=true
    otherClassList="w-100 d-flex ms-auto"
    otherLanguageSelect=true
    otherBtn=true
    otherBtnClassList="btn btn-sm btn-white rounded-pill"
    otherBtnText="Contact"
    otherBtnLink="/contact/"
%}
</header>
<!-- /header -->

{% include components/sections/services2/hero.html %}
{% include components/sections/services2/what-we-do.html %}
{% include components/sections/services2/video.html %}
{% include components/sections/services2/features.html %}
{% include components/sections/services2/pricing.html %}
{% include components/sections/services2/community.html %}

{% include components/footer/footer.html 
  style="default"
  bg_color="bg-dark"
  text_color="text-inverse"
  mt="mt-5 mt-md-16"
%}
</div>
