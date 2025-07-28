---
layout: default
title: Demo 28
permalink: /demo28/
custom_color: purple
custom_font: space
scroll_top_btn:
  enable: true

# Hero Section
hero:
  enable: true
  bg_class: "bg-gradient-blend"
  profile_image: /assets/img/photos/about28.jpg
  profile_image2x: /assets/img/photos/about28@2x.jpg
  greeting: "Hello! I'm Julia"
  title: I'm a corporate <em>brand designer</em> based in New York City.
  content: I'm very passionate about the work that I do, and if you are curious you can find my works on <a href="#" class="hover" style="color var(--bs-dribbble);">Dribbble</a>, my portfolio on <a href="#" class="hover" style="color var(--bs-behance);">Behance</a>, and my shots on <a href="#" class="hover" style="color var(--bs-instagram);">Instagram</a>.

# Portfolio Section
portfolio:
  

# Expertise Section
expertise:
  title: My areas of <em>expertise</em>
  subtitle: The full service I am offering is specifically designed to meet your business needs.
  text: Donec ullamcorper nulla non metus auctor fringilla. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam quis risus eget urna mollis ornare vel eu leo. Nullam quis risus eget urna mollis ornare vel eu leo. Maecenas faucibus mollis elit interdum. Duis mollis, est non commodo luctus, nisi erat ligula magna mollis.
  button_text: More Details
  button_url: "#"
  services:
    - icon: edit
      title: Content Marketing
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida.
      link: "#"
      link_text: Learn More
    - icon: team
      title: Social Engagement
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida.
      link: "#"
      link_text: Learn More
    - icon: lamp
      title: Identity & Branding
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida.
      link: "#"
      link_text: Learn More
    - icon: delivery-box
      title: Product Design
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida.
      link: "#"
      link_text: Learn More

# Results Section
results:
  title: I am <em>proud</em> of my results
  subtitle: I bring solutions to make life easier for our customers.
  counters:
    - icon: target
      value: 1000+
      label: Completed Projects
    - icon: medal
      value: 12
      label: Awards Won
    - icon: employees
      value: 99.7%
      label: Customer Satisfaction

# Testimonials Section
testimonials:
  

# About Section
about:
  image: /assets/img/photos/about28.jpg
  image2x: /assets/img/photos/about28@2x.jpg
  title: More <em>about</em> me
  subtitle: I'm Julia Sandbox, a corporate brand designer based in New York City. I'm very passionate about the work that I do.
  text1: Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Etiam porta sem malesuada magna mollis euismod. Vestibulum id ligula.
  text2: Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Aenean lacinia bibendum nulla sed consectetur. Curabitur blandit tempus porttitor. Lorem ipsum dolor sit amet, consectetur.
  button_text: Learn More
  button_url: "#"

# Process Section
process:
  title: My <em>working</em> process
  subtitle: Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Fusce dapibus, tellus ac cursus. Aenean eu leo quam.
  steps:
    - icon: lamp
      title: Concept
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida.
    - icon: puzzle
      title: Prepare
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida.
    - icon: pen-tool
      title: Retouch
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida.
    - icon: delivery-box
      title: Finalize
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida.

# Contact Section
contact:
  title: If you like what you see, <em>let's work</em> together.
  subtitle: Have any questions? Reach out to me from this contact form and I will get back to you shortly.
  icon: email-2
  form:
    action: /assets/php/contact.php
    fields:
      - id: form_name
        type: text
        name: name
        label: Name *
        placeholder: Jane
        required: true
        error_message: Please enter your name.
      - id: form_email
        type: email
        name: email
        label: Email *
        placeholder: jane.doe@example.com
        required: true
        error_message: Please provide a valid email address.
      - id: form_message
        type: textarea
        name: message
        label: Message *
        placeholder: Your message
        required: true
        error_message: Please enter your messsage.
    submit_text: Send message
---
<div class="content-wrapper">
<header class="wrapper bg-gradient-blend">
{% include components/navbar/navbar.html 
    wrapperClass=""
    classList="center-nav transparent position-absolute navbar-light caret-none pt-lg-0"
    centerNav=true
    logoAlt=true
    otherClassList="w-100 d-flex ms-auto"
    otherSocial=true
%}
</header>
<!-- /header -->

{% include components/sections/demo28/hero.html %}
{% include components/sections/demo28/portfolio.html %}
{% include components/sections/demo28/expertise.html %}
{% include components/sections/demo28/results.html %}
{% include components/sections/demo28/testimonials.html %}
{% include components/sections/demo28/about.html %}
{% include components/sections/demo28/process.html %}
{% include components/sections/demo28/contact.html %}

</div>

{% include components/footer/footer.html 
  style="centered" 
  bg_color="bg-light"
  text_color=""
  show_cta=false
  
%}
