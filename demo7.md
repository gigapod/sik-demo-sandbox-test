---
layout: default
title: Demo 7
permalink: /demo7/
custom_color: purple
custom_font: thicccboi
scroll_top_btn:
  enable: true 

# Hero Section
hero:
  title: Creative. Smart. Awesome.
  subtitle: We are an award winning web & mobile design agency that strongly believes in the power of creative ideas.
  buttons:
    - label: See Projects
      url: "#"
      class: btn btn-lg btn-primary rounded-pill mx-1
    - label: Contact Us
      url: "#"
      class: btn btn-lg btn-outline-primary rounded-pill mx-1
  image: /assets/img/illustrations/i12.png
  image2x: /assets/img/illustrations/i12@2x.png

# What We Do Section
what_we_do:
  title: What We Do?
  subtitle: The full service we are offering is specifically designed to meet your business needs.
  text: Donec ullamcorper nulla non metus auctor fringilla. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam quis risus eget urna mollis ornare vel eu leo. Nullam quis risus eget urna mollis ornare vel eu leo. Maecenas faucibus mollis elit interdum. Duis mollis, est non commodo luctus, nisi erat ligula.
  button_text: More Details
  button_url: "#"
  services:
    - image: /assets/img/photos/se1.jpg
      image2x: /assets/img/photos/se1@2x.jpg
      icon: uil uil-monitor
      icon_color: purple
      title: Web Design
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida.
      learn_more_url: "#"
    - image: /assets/img/photos/se2.jpg
      image2x: /assets/img/photos/se2@2x.jpg
      icon: uil uil-mobile-android
      icon_color: purple
      title: Mobile Design
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida.
      learn_more_url: "#"

# Community Section
community:
  title: Join Our Community
  subtitle: We have considered our business solutions to support you on every stage of your growth.
  text: Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Praesent commodo cursus magna, vel scelerisque nisl consectetur.
  counters:
    - icon: uil uil-presentation-check
      icon_color: purple
      number: 7518
      text: Projects Done
    - icon: uil uil-users-alt
      icon_color: red
      number: 3472
      text: Happy Customers
    - icon: uil uil-user-check
      icon_color: yellow
      number: 4537
      text: Expert Employees
    - icon: uil uil-trophy
      icon_color: aqua
      number: 2184
      text: Awards Won

# Projects Section
projects:
  title: Our Recent Projects
  

# Control Section
control:
  title: Have Perfect Control
  subtitle: We are focused on establishing long-term relationships with customers.
  text: Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus magna, vel scelerisque nisl consectetur et.
  features:
    - text: Aenean quam ornare. Curabitur blandit.
    - text: Nullam quis risus eget urna mollis ornare.
    - text: Etiam porta euismod malesuada mollis.
    - text: Vivamus sagittis lacus vel augue rutrum.
  image: /assets/img/illustrations/i9.png
  image2x: /assets/img/illustrations/i9@2x.png

# Why Choose Us Section
why_choose_us:
  title: Why Choose Us?
  subtitle: Find out everything you need to know about creating a business process model.
  image: /assets/img/illustrations/i17.png
  image2x: /assets/img/illustrations/i17@2x.png
  accordion:
    - title: Professional Design
      content: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel.
      active: true
    - title: Top-Notch Support
      content: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel.
      active: false
    - title: Header and Slider Options
      content: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel.
      active: false

# Testimonials Section
testimonials:
  title: Happy Customers
  
---
<div class="content-wrapper">
<header class="wrapper bg-soft-primary">
<!-- HEADER -->
{% include components/navbar/navbar-fancy.html 
    wrapperClass=""
    classList="fancy navbar-light navbar-bg-light caret-none"
    centerNav=true
    fancy=true
    logoAlt=true
    otherClassList="w-100 d-flex ms-auto"
    otherSocial=true
%}
</header>
<!-- /header -->

{% include components/sections/demo7/hero.html %}
{% include components/sections/demo7/what-we-do.html %}
{% include components/sections/demo7/community.html %}
{% include components/sections/demo7/projects.html %}
{% include components/sections/demo7/control.html %}
{% include components/sections/demo7/why-choose-us.html %}
{% include components/sections/demo7/testimonials.html %}

{% include components/footer/footer.html 
  style="three-column"
  container_padding="pt-15 pt-md-18 pb-7"
  bg_color="bg-light"
  newsletter_cta=true
%}
</div>