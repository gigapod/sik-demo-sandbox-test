---
layout: default
title: About
permalink: /about/
custom_color:
custom_font: 
scroll_top_btn:
  enable: true

# Header / Hero Section
hero:
  title: "Hello! This is Sandbox"
  subtitle: "A company turning ideas into beautiful things."
  bg_image: /assets/img/photos/bg12.jpg
  bg_color: "bg-gray"

# Who We Are Section
who_we_are:
  title: "Who Are We?"
  subtitle: "We are a digital and branding company that believes in the power of creative strategy and along with great design."
  text: "Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus magna, vel scelerisque nisl consectetur et."
  icon: "megaphone"
  list_items:
    - "Aenean eu leo quam ornare curabitur blandit tempus."
    - "Nullam quis risus eget urna mollis ornare donec elit."
    - "Etiam porta sem malesuada magna mollis euismod."
    - "Fermentum massa vivamus faucibus amet euismod."
  images:
    - src: /assets/img/photos/about2.jpg
      src2x: /assets/img/photos/about2@2x.jpg
    - src: /assets/img/photos/about3.jpg
      src2x: /assets/img/photos/about3@2x.jpg

# How It Works Section
how_it_works:
  title: "How It Works?"
  subtitle: "Find out everything you need to know and more about how we create our business process models."
  text: "Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Etiam porta sem malesuada magna mollis euismod. Nullam id dolor id nibh ultricies vehicula ut id elit. Nullam quis risus eget urna mollis ornare.\n\nNullam id dolor id nibh ultricies vehicula ut id elit. Vestibulum id ligula porta felis euismod semper. Aenean lacinia bibendum nulla sed consectetur. Sed posuere consectetur est at lobortis. Vestibulum id ligula porta felis."
  button:
    label: "Learn More"
    url: "#"
  steps:
    - number: "01"
      title: "Collect Ideas"
      text: "Nulla vitae elit libero pharetra augue dapibus."
    - number: "02" 
      title: "Data Analysis"
      text: "Vivamus sagittis lacus vel augue laoreet."
    - number: "03"
      title: "Finalize Product"
      text: "Cras mattis consectetur purus sit amet."

# Testimonials Section
testimonials:
  bg_color: "bg-soft-primary"
  image: /assets/img/photos/co1.png
  image2x: /assets/img/photos/co1@2x.png
  
# Team Section
team:
  title: "Save your time and money by choosing our professional team."
  subtitle: "Our Team"
  bg_color: "bg-light"
  
# Stats Section
stats:
  bg_color: "bg-soft-primary"
  items:
    - icon: check
      count: 7518
      label: "Completed Projects"
    - icon: user
      count: 3472
      label: "Satisfied Customers"
    - icon: briefcase-2
      count: 2184
      label: "Expert Employees"
    - icon: award-2
      count: 4523
      label: "Awards Won"

# Contact Section
contact:
  title: "Convinced yet? Let's make something great together."
  icon: "telemarketer"
  image: /assets/img/photos/about4.jpg
  image2x: /assets/img/photos/about4@2x.jpg
  info:
    - icon: "location-pin-alt"
      title: "Address"
      text: "Moonshine St. 14/05 Light City, London, United Kingdom"
    - icon: "phone-volume"
      title: "Phone"
      text: "00 (123) 456 78 90"
    - icon: "envelope"
      title: "E-mail"
      text: "sandbox@email.com"
      link: "mailto:sandbox@email.com"
---
<div class="content-wrapper">
<header class="wrapper bg-gray">
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

{% include components/sections/about/hero.html %}
{% include components/sections/about/who-we-are.html %}
{% include components/sections/about/testimonials.html %}
{% include components/sections/about/team.html %}
{% include components/sections/about/stats.html %}
{% include components/sections/about/contact.html %}

{% include components/footer/footer.html 
  style="default"
  container_padding="pt-16 pt-md-18 pb-13 pb-md-15"
  bg_color="bg-dark"
  text_color="text-inverse"
%}
</div>
