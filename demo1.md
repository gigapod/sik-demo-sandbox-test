---
layout: default
title: Demo 1
permalink: /demo1/
custom_color: yellow
custom_font: thicccboi
scroll_top_btn:
  enable: true

# Hero Section
hero:
  title: "Grow Your Business with Our Solutions."
  subtitle: "We help our clients to increase their website traffic, rankings and visibility in search results."
  button:
    label: "Try It For Free"
    url: "#"
  image: /assets/img/illustrations/i2.png
  image2x: /assets/img/illustrations/i2@2x.png

# What We Do Section
services:
  title: "The service we offer is specifically designed to meet your needs."
  subtitle: "What We Do?"
  items:
    - icon: search-2
      iconColor: "yellow"
      title: "SEO Services"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus cras justo."
      link: "#"
      linkClass: "link-yellow"
    - icon: browser
      iconColor: "red"
      title: "Web Design"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus cras justo."
      link: "#"
      linkClass: "link-red"
    - icon: chat-2
      iconColor: "green"
      title: "Social Engagement"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus cras justo."
      link: "#"
      linkClass: "link-green"
    - icon: megaphone
      iconColor: "blue"
      title: "Content Marketing"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus cras justo."
      link: "#"
      linkClass: "link-blue"

# Analyze Section
analyze:
  title: "Wonder how much faster your website can go? Easily check your SEO Score now."
  subtitle: "Analyze Now"
  text: "Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus magna, vel scelerisque nisl consectetur et."
  image: /assets/img/illustrations/i3.png
  image2x: /assets/img/illustrations/i3@2x.png

# Our Strategy Section
strategy:
  title: "Here are 3 working steps to organize our business projects."
  subtitle: "Our Strategy"
  text: "Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Etiam porta sem malesuada magna mollis euismod. Nullam id dolor id nibh ultricies vehicula ut id elit. Nullam quis risus eget urna mollis.\n\nNullam id dolor id nibh ultricies vehicula ut id elit. Vestibulum id ligula porta felis euismod semper. Aenean lacinia bibendum nulla sed consectetur."
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

# Why Choose Us Section
whychoose:
  title: "We bring solutions to make life easier for our clients."
  subtitle: "Why Choose Us?"
  image: /assets/img/illustrations/i6.png
  image2x: /assets/img/illustrations/i6@2x.png
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
  title: "Think unique and be innovative. Make a difference with Sandbox."
  subtitle: "Our Team"
  
# Solutions Section
solutions:
  title: "We make your spending stress-free for you to have the perfect control."
  subtitle: "Our Solutions"
  text: "Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus."
  image: /assets/img/illustrations/i8.png
  image2x: /assets/img/illustrations/i8@2x.png
  features:
    - text: "Aenean quam ornare. Curabitur blandit."
    - text: "Nullam quis risus eget urna mollis ornare."
    - text: "Etiam porta euismod malesuada mollis."
    - text: "Vivamus sagittis lacus vel augue rutrum."

# Testimonials Section testimonials are coming from json
testimonials:
  title: "Don't take our word for it. See what customers are saying about us."
  subtitle: "Our Community"
  text: "Aenean lacinia bibendum nulla sed consectetur. Praesent commodo cursus magna, vel scelerisque nisl consectetur et. Nulla vitae elit libero, a pharetra augue. Maecenas faucibus mollis interdum. Vestibulum id ligula porta felis euismod."
  button:
    label: "All Testimonials"
    url: "#"
  

# Pricing Section use pricing_plans.json
pricing:
  title: "We offer great and premium prices."
  subtitle: "Our Pricing"
  text: "Enjoy a <a href=\"#\" class=\"hover\">free 30-day trial</a> and experience the full service. No credit card required!"
  button:
    label: "See All Prices"
    url: "#"
  

# Let's Talk Section
lets_talk:
  title: "Let's make something great together. We are trusted by over 5000+ clients."
  subtitle: "Let's Talk"
  text: "Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Maecenas faucibus mollis interdum. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus."
  button:
    label: "Join Us"
    url: "#"
  image: /assets/img/illustrations/i5.png
  image2x: /assets/img/illustrations/i5@2x.png

# Clients Section is from clients.json
clients:
 
---
<div class="content-wrapper">
<header class="wrapper bg-soft-primary">
{% include components/navbar/navbar.html 
    classList="navbar-light navbar-light"
    logoAlt=true
    otherClassList="w-100 d-flex ms-auto"
    otherLanguageSelect=true
    otherInfo=true
%}
</header>
<!-- /header -->

{% include components/sections/demo1/hero.html %}
{% include components/sections/demo1/services.html %}
{% include components/sections/demo1/analyze.html %}
{% include components/sections/demo1/strategy.html %}
{% include components/sections/demo1/whychoose.html %}
{% include components/sections/demo1/team.html %}
{% include components/sections/demo1/solutions.html %}
{% include components/sections/demo1/testimonials.html %}
{% include components/sections/demo1/pricing.html %}
{% include components/sections/demo1/lets-talk.html %}
{% include components/sections/demo1/clients.html %}

{% include components/footer/footer.html 
  style="default"
  bg_color="bg-navy"
  text_color="text-inverse"
  cta=true
  cta_title="Join our community by using our services and grow your business."
  cta_button_text="Try It For Free"
  cta_button_url="#"
%}
</div>
