---
layout: default
title: One Page
permalink: /onepage/
custom_color: blue
custom_font: thicccboi
scroll_top_btn:
  enable: true

# Hero Section
hero:
  title: "Creative. Smart. Awesome."
  subtitle: "We are an award winning web & mobile design agency that strongly believes in the power of creative ideas."
  image: /assets/img/illustrations/i8.png
  image2x: /assets/img/illustrations/i8@2x.png 2x

# Services Section
services:
  title: "The full service we are offering is specifically designed to meet your business needs and projects."
  subtitle: "Our Services"
  text: "Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Praesent commodo cursus magna, vel scelerisque nisl consectetur duis mollis commodo."
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
  items:
    - icon: megaphone
      iconColor: "text-blue"
      title: "Marketing"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus. Cras justo cum sociis natoque magnis."
    - icon: target
      iconColor: "text-green"
      title: "Strategy"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus. Cras justo cum sociis natoque magnis."
    - icon: settings-3
      iconColor: "text-yellow"
      title: "Development"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus. Cras justo cum sociis natoque magnis."
    - icon: bar-chart
      iconColor: "text-orange"
      title: "Data Analysis"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus. Cras justo cum sociis natoque magnis."

# Process Section
process:
  title: "Everything you need on creating a business process."
  subtitle: "How It Works?"
  image: /assets/img/illustrations/i3.png
  image2x: /assets/img/illustrations/i3@2x.png 2x
  steps:
    - icon: light-bulb
      iconColor: "text-blue"
      title: "Collect Ideas"
      text: "Nulla vitae elit libero pharetra augue dapibus."
    - icon: pie-chart-2
      iconColor: "text-green"
      title: "Data Analysis"
      text: "Vivamus sagittis lacus augue laoreet vel."
    - icon: design
      iconColor: "text-yellow"
      title: "Magic Touch"
      text: "Cras mattis consectetur purus sit amet."

# Why Choose Us Section
whychoose:
  title: "A few reasons why our valued customers choose us."
  subtitle: "Why Choose Us?"
  image: /assets/img/illustrations/i2.png
  image2x: /assets/img/illustrations/i2@2x.png 2x
  accordion:
    - title: "Professional Design"
      text: "Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel."
      show: true
    - title: "Top-Notch Support"
      text: "Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel."
      show: false
    - title: "Header and Slider Options"
      text: "Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel."
      show: false

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
  title: "Got any questions? Don't hesitate to get in touch."
  subtitle: "Get In Touch"
  image: /assets/img/illustrations/i4.png
  image2x: /assets/img/illustrations/i4@2x.png 2x
  

# Clients Section
clients:
  brands:
    - image: /assets/img/brands/c1.png
    - image: /assets/img/brands/c2.png
    - image: /assets/img/brands/c3.png
    - image: /assets/img/brands/c4.png
    - image: /assets/img/brands/c5.png
    - image: /assets/img/brands/c6.png

# Contact Section
contact:
  title: "Got any questions? Don't hesitate to get in touch."
  subtitle: "Get In Touch"
  image: /assets/img/illustrations/i5.png
  image2x: /assets/img/illustrations/i5@2x.png 2x
  info:
    - icon: "uil-location-pin-alt"
      title: "Address"
      text: "Moonshine St. 14/05 Light City, London"
    - icon: "uil-phone-volume"
      title: "Phone"
      text: "00 (123) 456 78 90"
    - icon: "uil-envelope"
      title: "E-mail"
      text: "sandbox@email.com"

# Footer section
footer:
  enable: true
  style: "dark"
  bg_color: "bg-dark"
  text_color: "text-inverse"
---
<div class="content-wrapper">
<header class="wrapper bg-gray">
{% include components/navbar/navbar.html 
    wrapperClass="bg-gray"
    classList="navbar-expand-lg center-nav transparent navbar-light"
    centerNav=true
    logoAlt=true
    otherClassList="w-100 d-flex ms-auto"
    otherLanguageSelect=true
    otherBtn=true
    otherBtnClassList="btn btn-sm btn-primary rounded-pill"
    otherBtnText="Contact"
    otherBtnLink="/contact/"
    onePage=true
%}
</header>
<!-- /header -->

{% include components/sections/onepage/hero.html %}
{% include components/sections/onepage/services.html %}
{% include components/sections/onepage/process.html %}
{% include components/sections/onepage/about.html %}
{% include components/sections/onepage/testimonials.html %}
{% include components/sections/onepage/contact.html %}

{% include components/footer/footer.html 
  style="default"
  bg_color="bg-dark" 
  text_color="text-inverse"
%}
</div>
