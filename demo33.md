---
layout: default
title: Demo 33
permalink: /demo33/
custom_color: navy
custom_font: space
scroll_top_btn:
  enable: true

# Hero Section
hero:
  wrapper_classes: "mx-xxl-11 overflow-hidden"
  background_image: "/assets/img/photos/bg23.png"
  has_shapes: true
  title: "👋 Hello! I'm <img class=\"d-inline w-12 mx-1\" src=\"/assets/img/avatars/avatar.png\" alt=\"\"> Camille, a product designer."
  subtitle: "I'm very passionate about the work that I do, and if you are curious you can find my works on <a href=\"#\" class=\"hover\" style=\"color: var(--bs-dribbble);\">Dribbble</a>, my portfolio on <a href=\"#\" class=\"hover\" style=\"color: var(--bs-behance);\">Behance</a>."
  button:
    text: "See My Works"
    url: "#"

# Services Section
services:
  title: "The service I offer is specifically designed to meet your needs."
  description: "Cras mattis consectetur purus sit amet fermentum. Donec ullamcorper nulla non metus auctor fringilla. Integer posuere erat a ante venenatis dapibus posuere velit aliquet."
  button:
    text: "More Details"
    url: "#"
  service_items:
    - icon: "search-2.svg"
      color: "fuchsia"
      title: "User Research"
      text: "Duis mollis gravida commodo id luctus erat porttitor ligula, nulla non metus auctor eget lacinia odio sem aget elit."
    - icon: "puzzle-2.svg"
      color: "aqua"
      title: "Strategy & Planning"
      text: "Duis mollis gravida commodo id luctus erat porttitor ligula, nulla non metus auctor eget lacinia odio sem aget elit."
    - icon: "smartphone.svg"
      color: "yellow"
      title: "App Design"
      text: "Duis mollis gravida commodo id luctus erat porttitor ligula, nulla non metus auctor eget lacinia odio sem aget elit."
    - icon: "design.svg"
      color: "leaf"
      title: "Brand Design"
      text: "Duis mollis gravida commodo id luctus erat porttitor ligula, nulla non metus auctor eget lacinia odio sem aget elit."
    - icon: "video-editing.svg"
      color: "orange"
      title: "Motion Graphic"
      text: "Duis mollis gravida commodo id luctus erat porttitor ligula, nulla non metus auctor eget lacinia odio sem aget elit."
    - icon: "browser.svg"
      color: "grape"
      title: "Web Design"
      text: "Duis mollis gravida commodo id luctus erat porttitor ligula, nulla non metus auctor eget lacinia odio sem aget elit."

# Projects Section
projects:
  title: "Check out some of my latest projects with creative ideas."
  button:
    text: "See All Projects"
    url: "#"
  

# Testimonials Section
testimonials:
  background_image: "/assets/img/photos/bg23.png"
  title: "Don't take our word for it. See what customers are saying about us."
  

# About Section
about:
  image: "/assets/img/avatars/avatar.jpg"
  image2x: "/assets/img/avatars/avatar@2x.jpg"
  title: "More about me"
  lead: "👋 Hello! I'm Camille, a multidisciplinary product designer 🧸 based in New York City 🚕. I'm very passionate about the work 💌 that I do."
  description:
    - "Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh ut fermentum massa justo sit amet risus."
    - "Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Aenean lacinia bibendum nulla sed consectetur."
  button:
    text: "Learn More"
    url: "#"
  
  # Experience Section (part of About)
  experience:
    title: "My experiences"
    lead: "I've had the pleasure to work with companies 🏢 across a variety of industries 🏛️ I'm always interested in new ✨ and exciting adventures 🧨"
    button:
      text: "Download Resume"
      url: "#"
    items:
      - period: "Nov 2017 - Present"
        title: "Creative Director at Malory House"
        description: "Nullam vel sem. Nullam vel sem. Integer ante arcu, accumsan a consectetuer eget, posuere ut, mauris. Donec orci lectus, aliquam ut, faucibus non euismod id nulla."
      - period: "Sep 2015 - Apr 2017"
        title: "Senior Developer at Longwave Studio"
        description: "Donec vitae sapien ut libero venenatis faucibus. ullam dictum felis eu pede mollis pretium. Pellentesque ut neque."
      - period: "May 2011 - Sep 2015"
        title: "Junior Developer at Webpaint Media"
        description: "Cras mattis consectetur purus sit amet fermentum. Donec ullamcorper nulla non metus auctor fringilla. Integer posuere erat a ante venenatis dapibus posuere velit aliquet."

# CTA Section
cta:
  wrapper_classes: "mx-xxl-11 overflow-hidden"
  background_image: "/assets/img/photos/bg23.png"
  has_shapes: true
  title: "Got a 👾 project in mind? Let's work together. ✌️"
  subtitle: "I bring rapid solutions to make the life of my clients easier. Have any questions? Reach out to me and I will get back to you shortly."
  button:
    text: "Contact Me"
    url: "#"
---
<div class="content-wrapper">
<header class="wrapper">
{% include components/navbar/navbar.html 
    classList="center-nav transparent navbar-light caret-none"
    logoAlt="logo-dark"
    otherClassList="w-100 d-flex ms-auto"
    otherSocial=true
%}

</header>
<!-- /header -->

{% include components/sections/demo33/hero.html %}
{% include components/sections/demo33/services.html %}
{% include components/sections/demo33/projects.html %}
{% include components/sections/demo33/testimonials.html %}
{% include components/sections/demo33/about.html %}
{% include components/sections/demo33/cta.html %}

{% include components/footer/footer.html 
  style="default"

%}
</div>
