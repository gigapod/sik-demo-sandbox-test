---
layout: default
title: Demo 15
permalink: /demo15/
custom_color: default
scroll_top_btn:
  enable: true

# Hero Section
hero:
  slides:
    - background: /assets/img/photos/bg7.webp
      title: We bring solutions to make life easier.
      subtitle: We are a creative company that focuses on long term relationships with customers.
      button:
        label: Read More
        url: "#"
        class: btn btn-lg btn-outline-white rounded-pill
      position: left
      animation: true
    - background: /assets/img/photos/bg8.webp
      title: We are trusted by over a million customers.
      subtitle: Here a few reasons why our customers choose us.
      video_url: /assets/media/movie.mp4
      position: center
      animation: true
    - background: /assets/img/photos/bg9.webp
      title: Just sit and relax.
      subtitle: We make sure your spending is stress free so that you can have the perfect control.
      button:
        label: Contact Us
        url: "#"
        class: btn btn-lg btn-outline-white rounded-pill
      position: right
      animation: true

# About Section
about:
  icon: /assets/img/icons/lineal/megaphone.svg
  title: Who Are We?
  subtitle: We are a digital and branding company that believes in the power of creative strategy and along with great design.
  text: Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus magna, vel scelerisque nisl consectetur et.
  features:
    - text: Aenean eu leo quam ornare curabitur blandit tempus.
    - text: Nullam quis risus eget urna mollis ornare donec elit.
    - text: Etiam porta sem malesuada magna mollis euismod.
    - text: Fermentum massa vivamus faucibus amet euismod.
  images:
    - image: /assets/img/photos/about2.webp
      image2x: /assets/img/photos/about2@2x.webp
    - image: /assets/img/photos/about3.webp
      image2x: /assets/img/photos/about3@2x.webp

# Working Steps Section
working_steps:
  title: Here are 3 working steps to organize our business projects.
  icon: /assets/img/icons/lineal/list.svg
  steps:
    - number: "01"
      title: Collect Ideas
      text: Nulla vitae elit libero pharetra augue dapibus.
    - number: "02"
      title: Data Analysis
      text: Vivamus sagittis lacus vel augue laoreet.
    - number: "03"
      title: Finalize Product
      text: Cras mattis consectetur purus sit amet.
  how_it_works:
    title: How It Works?
    subtitle: Find out everything you need to know and more about how we create our business process models.
    text1: Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Etiam porta sem malesuada magna mollis euismod. Nullam id dolor id nibh ultricies vehicula ut id elit. Nullam quis risus eget urna mollis ornare.
    text2: Nullam id dolor id nibh ultricies vehicula ut id elit. Vestibulum id ligula porta felis euismod semper. Aenean lacinia bibendum nulla sed consectetur. Sed posuere consectetur est at lobortis. Vestibulum id ligula porta felis.
    button:
      label: Learn More
      url: "#"
      class: btn btn-primary rounded-pill mb-0

# Testimonials Section
testimonials:
  image: /assets/img/photos/co1.png
  image2x: /assets/img/photos/co1@2x.png
  

# Team Section
team:
  title: Save your time and money by choosing our professional team.
  icon: /assets/img/icons/lineal/team.svg
  
# Stats Section
stats:
  counters:
    - icon: /assets/img/icons/lineal/check.svg
      count: 7518
      text: Completed Projects
    - icon: /assets/img/icons/lineal/user.svg
      count: 3472
      text: Satisfied Customers
    - icon: /assets/img/icons/lineal/briefcase-2.svg
      count: 2184
      text: Expert Employees
    - icon: /assets/img/icons/lineal/award-2.svg
      count: 4523
      text: Awards Won

# Contact Section
contact:
  title: Convinced yet? Let's make something great together.
  icon: /assets/img/icons/lineal/telemarketer.svg
  image: /assets/img/photos/about4..webp
  image2x: /assets/img/photos/about4@2x..webp
  contact_info:
    - icon: uil uil-location-pin-alt
      title: Address
      text: Moonshine St. 14/05 Light City,<br />London, United Kingdom
    - icon: uil uil-phone-volume
      title: Phone
      text: 00 (123) 456 78 90
    - icon: uil uil-envelope
      title: E-mail
      text: sandbox@email.com
      link: mailto:sandbox@email.com

# Community Section
community:
  title: Join Our Community
  subtitle: We are trusted by over 5000+ clients. Join them by using our services and grow your business.
  icon: /assets/img/icons/lineal/puzzle-2.svg
---
<div class="content-wrapper">
<header class="wrapper bg-soft-primary">
{% include components/navbar/navbar.html 
    classList="center-nav transparent position-absolute navbar-dark caret-none"
    logoLight=true
    logoBoth=true
    otherClassList="w-100 d-flex ms-auto"
    otherSearch=true
    otherInfo=true
%}
</header>
<!-- /header -->

{% include components/sections/demo15/hero.html %}
{% include components/sections/demo15/about.html %}
{% include components/sections/demo15/working-steps.html %}
{% include components/sections/demo15/testimonials.html %}
{% include components/sections/demo15/team.html %}
{% include components/sections/demo15/stats.html %}
{% include components/sections/demo15/contact.html %}
{% include components/sections/demo15/community.html %}

{% include components/footer/footer.html 
  style="default" 
  bg_color="bg-dark"
  text_color="text-inverse"
%}
</div>
