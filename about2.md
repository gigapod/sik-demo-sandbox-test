---
layout: default
title: About Us
permalink: /about2/
custom_color:
custom_font: 
scroll_top_btn:
  enable: true

# Header / Hero Section
hero:
  title: "About Us"
  subtitle: "A company turning ideas into beautiful things."
  bg_color: "bg-soft-primary"

# Services Section
services:
  image: /assets/img/illustrations/i8.png
  image2x: /assets/img/illustrations/i8@2x.png
  progress_list:
    - name: "Marketing"
      value: 100
      color: "blue"
    - name: "Strategy"
      value: 80
      color: "green"
    - name: "Development"
      value: 85
      color: "yellow"
    - name: "Data Analysis"
      value: 90
      color: "orange"
  title: "The full service we are offering is specifically designed to meet your business needs and projects."
  text: "Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Praesent commodo cursus magna, vel scelerisque nisl consectetur duis mollis commodo."
  items:
    - icon: "megaphone"
      icon_color: "blue"
      title: "Marketing"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus. Cras justo cum sociis natoque magnis."
    - icon: "target"
      icon_color: "green"
      title: "Strategy"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus. Cras justo cum sociis natoque magnis."
    - icon: "settings-3"
      icon_color: "yellow"
      title: "Development"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus. Cras justo cum sociis natoque magnis."
    - icon: "bar-chart"
      icon_color: "orange"
      title: "Data Analysis"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus. Cras justo cum sociis natoque magnis."

# How It Works Section
how_it_works:
  title: "How It Works?"
  subtitle: "Everything you need on creating a business process."
  image: /assets/img/illustrations/i3.png
  image2x: /assets/img/illustrations/i3@2x.png
  steps:
    - icon: "light-bulb"
      icon_color: "blue"
      title: "Collect Ideas"
      text: "Nulla vitae elit libero pharetra augue dapibus."
    - icon: "pie-chart-2"
      icon_color: "green"
      title: "Data Analysis"
      text: "Vivamus sagittis lacus vel augue laoreet vel."
    - icon: "design"
      icon_color: "yellow"
      title: "Magic Touch"
      text: "Cras mattis consectetur purus sit amet."

# Why Choose Us Section
why_choose_us:
  title: "Why Choose Us?"
  subtitle: "A few reasons why our valued customers choose us."
  image: /assets/img/illustrations/i2.png
  image2x: /assets/img/illustrations/i2@2x.png
  accordion:
    - title: "Professional Design"
      content: "Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel."
      active: true
    - title: "Top-Notch Support"
      content: "Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel."
      active: false
    - title: "Header and Slider Options"
      content: "Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel."
      active: false

# Team Section
team:
  title: "Save your time and money by choosing our professional team."
  subtitle: "Meet the Team"
  text: "Donec id elit non mi porta gravida at eget metus. Morbi leo risus, porta ac consectetur ac, vestibulum at eros tempus porttitor."
  button:
    label: "See All Members"
    url: "#"
 

# Testimonials Section
testimonials:
  image: /assets/img/illustrations/i4.png
  image2x: /assets/img/illustrations/i4@2x.png
  bg_color: "bg-gray"
  

# Brands Section
brands:
 

# Contact Section
contact:
  title: "Get In Touch"
  subtitle: "Got any questions? Don't hesitate to get in touch."
  image: /assets/img/illustrations/i5.png
  image2x: /assets/img/illustrations/i5@2x.png
  info:
    - icon: "location-pin-alt"
      title: "Address"
      text: "Moonshine St. 14/05 Light City, London"
    - icon: "phone-volume"
      title: "Phone"
      text: "00 (123) 456 78 90"
    - icon: "envelope"
      title: "E-mail"
      text: "sandbox@email.com"
      link: "mailto:sandbox@email.com"
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

{% include components/sections/about2/hero.html %}
{% include components/sections/about2/services.html %}
{% include components/sections/about2/how-it-works.html %}
{% include components/sections/about2/team.html %}
{% include components/sections/about2/testimonials.html %}
{% include components/sections/about2/brands.html %}
{% include components/sections/about2/contact.html %}

{% include components/footer/footer.html 
  style="dark"
  bg_color="bg-dark"
  text_color="text-inverse"
%}
</div>
