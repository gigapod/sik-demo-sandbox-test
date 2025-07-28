---
layout: default
title: Demo 4
permalink: /demo4/
custom_color: violet
custom_font: dm
scroll_top_btn:
  enable: true 

# Hero Section
hero:
  title: Just sit & relax while we take care of your business needs.
  subtitle: We make your spending stress-free for you to have the perfect control.
  buttons:
    - label: Explore Now
      url: "#"
      class: btn btn-lg btn-primary rounded-pill me-2
    - label: Contact Us
      url: "#"
      class: btn btn-lg btn-outline-primary rounded-pill
  image: /assets/img/photos/about16.webp
  image_position: right
  min_height: min-vh-70 

# About Section
about:
  title: We bring solutions to make life easier for our customers.
  text: Nulla vitae elit libero, a pharetra augue. Aenean lacinia bibendum nulla sed consectetur. Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Vestibulum id ligula porta felis euismod semper. Vestibulum id ligula.
  features:
    - text: Aenean quam ornare curabitur blandit consectetur.
    - text: Nullam quis risus eget urna mollis ornare aenean leo.
    - text: Etiam porta euismod malesuada mollis nisl ornare sem.
    - text: Vivamus sagittis lacus augue rutrum maecenas.
  experience_counter:
    number: 20+
    text: Year Experience

# Services Section
services:
  items:
    - icon: telephone-3
      title: 24/7 Support
      text: Duis mollis gravida commodo id luctus erat porttitor ligula, eget lacinia odio sem aget elit nullam quis risus eget.
    - icon: shield
      title: Secure Payments
      text: Duis mollis gravida commodo id luctus erat porttitor ligula, eget lacinia odio sem aget elit nullam quis risus eget.
    - icon: cloud-computing-3
      title: Daily Updates
      text: Duis mollis gravida commodo id luctus erat porttitor ligula, eget lacinia odio sem aget elit nullam quis risus eget.
    - icon: analytics
      title: Market Research
      text: Duis mollis gravida commodo id luctus erat porttitor ligula, eget lacinia odio sem aget elit nullam quis risus eget.
    - icon: settings
      title: System Integration
      text: Duis mollis gravida commodo id luctus erat porttitor ligula, eget lacinia odio sem aget elit nullam quis risus eget.
    - icon: earth
      title: SEO Services
      text: Duis mollis gravida commodo id luctus erat porttitor ligula, eget lacinia odio sem aget elit nullam quis risus eget.

# Why Choose Us Section
why_choose_us:
  title: A few reasons why our valued customers choose us.
  accordion:
    - title: Professional Design
      content: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel scelerisque nisl consectetur et. Cum sociis natoque penatibus et magnis dis parturient montes.
      active: true
    - title: Top-Notch Support
      content: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel scelerisque nisl consectetur et. Cum sociis natoque penatibus et magnis dis parturient montes.
    - title: Header and Slider Options
      content: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel scelerisque nisl consectetur et. Cum sociis natoque penatibus et magnis dis parturient montes.

# Video Section
video:
  title: Find out everything you need to know about creating a business process model.
  video_url: /assets/media/movie.mp4
  background_image: /assets/img/photos/bg1.webp

# Team Section
team:
  title: We are proud of our creative team
  subtitle: Just sit back and relax while we take care of your business needs.
  stats:
    - icon: check
      number: 7518
      text: Completed Projects
    - icon: user
      number: 3472
      text: Happy Customers
    - icon: briefcase-2
      number: 2184
      text: Expert Employees

# Testimonials Section items from testimonial json
testimonials:
  title: What People Say About Us
  subtitle: Don't take our word for it. See what customers are saying about us.
  satisfied_counter:
    number: 5000+
    text: Satisfied Customers
  

# Clients Section from client json
clients:

# Contact Section
contact:
  title: Let's Talk
  subtitle: Let's make something great together. We are trusted by over 5000+ clients. Join them by using our services and grow your business.
  text: Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Maecenas faucibus mollis interdum. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus.
  button_text: Join Us
  button_url: "#"
  image: /assets/img/photos/tm1.webp
---
<div class="content-wrapper">
<!-- HEADER -->
{% include components/navbar/navbar.html 
    wrapperClass=""
    classList="center-nav transparent navbar-light caret-none pt-lg-0"
    centerNav=true
    logoAlt=true
    otherClassList="w-100 d-flex ms-auto"
    otherSocial=true
%}
<!-- /header -->

{% include components/sections/demo4/hero.html %}
{% include components/sections/demo4/about.html %}
{% include components/sections/demo4/services.html %}
{% include components/sections/demo4/why-choose-us.html %}
{% include components/sections/demo4/video.html %}
{% include components/sections/demo4/team.html %}
{% include components/sections/demo4/testimonials.html %}
{% include components/sections/demo4/clients.html %}

</div>
{% include components/footer/footer.html 
  style="centered" 
  bg_color="bg-soft-primary"
  text_color=""
  show_cta=true

  
%}