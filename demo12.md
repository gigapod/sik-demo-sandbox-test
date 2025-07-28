---
layout: default
title: Demo 12
permalink: /demo12/
custom_color: orange
custom_font: thicccboi
scroll_top_btn:
  enable: true

# Modal Popup
modal:
  enabled: true
  id: modal-02
  image: /assets/img/illustrations/i7.png
  image2x: /assets/img/illustrations/i7@2x.png
  title: Join the mailing list and get %10 off
  text: Nullam quis risus eget urna mollis ornare vel eu leo. Donec ullamcorper nulla non metus auctor fringilla.

# Hero Section
hero:
  title: Creative. Smart. Awesome.
  subtitle: We specialize in web, mobile and identity design. We love to turn ideas into beautiful things.
  buttons:
    - label: See Projects
      url: "#"
      class: btn btn-primary rounded me-2
    - label: Learn More
      url: "#"
      class: btn btn-yellow rounded
  image: /assets/img/illustrations/i6.png
  image2x: /assets/img/illustrations/i6@2x.png

# Services Section
services:
  services_items:
    - icon: /assets/img/icons/lineal/browser.svg
      color: yellow
      title: Content Marketing
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus cras justo.
      url: "#"
    - icon: /assets/img/icons/lineal/chat-2.svg
      color: green
      title: Social Engagement
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus cras justo.
      url: "#"
    - icon: /assets/img/icons/lineal/id-card.svg
      color: orange
      title: Identity & Branding
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus cras justo.
      url: "#"
    - icon: /assets/img/icons/lineal/gift.svg
      color: blue
      title: Product Design
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus cras justo.
      url: "#"

# Process Section
process:
  title: Our three process steps on creating awesome projects.
  image: /assets/img/illustrations/i8.png
  image2x: /assets/img/illustrations/i8@2x.png
  steps:
    - number: 1
      title: Collect Ideas
      text: Nulla vitae elit libero pharetra augue dapibus. Praesent commodo cursus. Donec ullamcorper nulla non metus.
    - number: 2
      title: Data Analysis
      text: Vivamus sagittis lacus vel augue laoreet. Etiam porta sem malesuada magna auctor fringilla augue.
    - number: 3
      title: Finalize Product
      text: Cras mattis consectetur purus sit amet. Aenean lacinia bibendum nulla sed. Nulla vitae elit libero pharetra.

# Why Choose Us Section
why_choose:
  title: Few reasons why our valued customers choose us.
  image: /assets/img/illustrations/i2.png
  image2x: /assets/img/illustrations/i2@2x.png
  accordion_items:
    - title: Professional Design
      content: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel.
      active: true
    - title: Top-Notch Support
      content: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel.
      active: false
    - title: Header and Slider Options
      content: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel.
      active: false

# Projects Section
projects:
  title: We are proud of our works
  subtitle: We bring solutions to make life easier for our customers.
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

# Testimonials Section
testimonials:
  

# Portfolio Section
portfolio:
  title: Check out some of our recent projects below.
  subtitle: We love to turn ideas into beautiful things.
  

# Contact Section
contact:
  title: Got any questions? Don't hesitate to get in touch.
  image: /assets/img/illustrations/i5.png
  image2x: /assets/img/illustrations/i5@2x.png
  contact_info:
    - icon: uil uil-location-pin-alt
      title: Address
      text: Moonshine St. 14/05 Light City, London
    - icon: uil uil-phone-volume
      title: Phone
      text: 00 (123) 456 78 90
    - icon: uil uil-envelope
      title: E-mail
      text: sandbox@email.com
      link: mailto:sandbox@email.com
---
<div class="content-wrapper">
<header class="wrapper bg-soft-primary">
{% include components/navbar/navbar-extended.html 
otherLanguageSelect=true

    
%} 
</header>
<!-- /header -->

{% include components/sections/demo12/modal/popup.html 
    id=page.modal.id
    image=page.modal.image
    image2x=page.modal.image2x
    title=page.modal.title
    text=page.modal.text
%}

{% include components/sections/demo12/hero.html %}
{% include components/sections/demo12/services.html %}
{% include components/sections/demo12/process.html %}
{% include components/sections/demo12/why-choose.html %}
{% include components/sections/demo12/counter.html %}
{% include components/sections/demo12/testimonials.html %}
{% include components/sections/demo12/portfolio.html %}
{% include components/sections/demo12/contact.html %}

{% include components/footer/footer.html 
  style="light"
%}
</div>
