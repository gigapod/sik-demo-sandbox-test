---
layout: default
title: Demo 26
permalink: /demo26/
custom_color: grape
custom_font: urbanist
scroll_top_btn:
  enable: true

# Hero Section
hero:
  title: "Grow Your Business with <br class=\"d-none d-md-block d-lg-none\" /><span class=\"text-primary\">Our Marketing Solutions</span>"
  subtitle: "We help our clients to increase their website <br class=\"d-none d-md-block d-lg-none\" /> traffic, rankings and visibility in search results."
  buttons:
    - label: "Try it for Free"
      url: "#"
      class: "btn btn-lg btn-grape rounded"
    - label: "Explore Now"
      url: "#"
      class: "btn btn-lg btn-outline-grape rounded"
  image: /assets/img/illustrations/3d11.png
  image2x: /assets/img/illustrations/3d11@2x.png
  bg_image: /assets/img/photos/clouds.png

# Services Section
services:
  title_tag: "What We Do?"
  title: "The full service we are offering is specifically designed to meet your business needs."
  service_items:
    - icon: globe-2
      title: "SEO Services"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida eget metus cras justo."
      link: "#"
      link_text: "Learn More"
    - icon: code
      title: "Web Design"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida eget metus cras justo."
      link: "#"
      link_text: "Learn More"
    - icon: team
      title: "Social Engagement"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida eget metus cras justo."
      link: "#"
      link_text: "Learn More"
    - icon: devices
      title: "App Development"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida eget metus cras justo."
      link: "#"
      link_text: "Learn More"

# Why Choose Us Section
why_choose:
  title_tag: "Why Choose Us?"
  title: "So here a few reasons why our valued customers choose us."
  image: /assets/img/illustrations/3d8.png
  image2x: /assets/img/illustrations/3d8@2x.png
  features:
    - icon: lamp
      title: "Creativity"
      text: "Curabitur blandit lacus porttitor ridiculus mus."
    - icon: bulb
      title: "Innovative Thinking"
      text: "Curabitur blandit lacus porttitor ridiculus mus."
    - icon: puzzle
      title: "Rapid Solutions"
      text: "Curabitur blandit lacus porttitor ridiculus mus."
    - icon: headphone
      title: "Top-Notch Support"
      text: "Curabitur blandit lacus porttitor ridiculus mus."

# Solutions Section
solutions:
  title_tag: "Our Solutions"
  title: "Just sit & relax while we take care of your business needs."
  text: "Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus. Maecenas sed diam eget risus varius blandit sit amet non magna. Praesent commodo cursus magna."
  image: /assets/img/illustrations/3d5.png
  image2x: /assets/img/illustrations/3d5@2x.png
  stats:
    - value: "99.7%"
      label: "Customer Satisfaction"
    - value: "4x"
      label: "New Visitors"

# Testimonials Section
testimonials:
  title_tag: "Happy Customers"
  title: "Don't take our word for it. See what customers are saying about us."
  image: /assets/img/photos/about28.jpg
  image2x: /assets/img/photos/about28@2x.jpg
  

# Pricing Section
pricing:
  title_tag: "Our Pricing"
  title: "We offer great and premium prices."
  subtitle: "Enjoy a <a href=\"#\" class=\"hover\">free 30-day trial</a> and experience the full service. No credit card required!"
  button_text: "See All Prices"
  button_url: "#"
  plans:
    - name: "Premium Plan"
      monthly_price: "19"
      yearly_price: "199"
      features:
        - text: "<strong>5</strong> Projects"
        - text: "<strong>100K</strong> API Access"
        - text: "<strong>200MB</strong> Storage"
        - text: "Weekly <strong>Reports</strong>"
        - text: "7/24 <strong>Support</strong>"
      button_text: "Choose Plan"
      button_url: "#"
      popular: false
    - name: "Corporate Plan"
      monthly_price: "49"
      yearly_price: "499"
      features:
        - text: "<strong>20</strong> Projects"
        - text: "<strong>300K</strong> API Access"
        - text: "<strong>500MB</strong> Storage"
        - text: "Weekly <strong>Reports</strong>"
        - text: "7/24 <strong>Support</strong>"
      button_text: "Choose Plan"
      button_url: "#"
      popular: true

# Let's Talk Section
lets_talk:
  title_tag: "Let's Talk"
  title: "Let's make something great together. We are trusted by over 5000+ clients."
  text: "Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Maecenas faucibus mollis interdum. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus."
  button_text: "Join Us"
  button_url: "#"
  image: /assets/img/illustrations/3d3.png
  image2x: /assets/img/illustrations/3d3@2x.png

# Analyze Section
analyze:
  title_tag: "Analyze Now"
  title: "Wonder how much faster your website can go? Easily check your SEO Score now."
  button_text: "Analyze"
  bg_image: /assets/img/photos/clouds.png

---
<div class="content-wrapper">
<header class="wrapper bg-soft-primary">
{% include components/navbar/navbar.html 
    classList="navbar-light navbar-light"
    logoAlt=true
    otherClassList="w-100 d-flex ms-auto"
    otherBtn=true
    otherBtnClassList="btn btn-sm btn-primary rounded"
    otherBtnText="Free Trial"
    otherBtnLink="#"
%}
</header>
<!-- /header -->

{% include components/sections/demo26/hero.html %}
{% include components/sections/demo26/services.html %}
{% include components/sections/demo26/why-choose.html %}
{% include components/sections/demo26/solutions.html %}
{% include components/sections/demo26/testimonials.html %}
{% include components/sections/demo26/pricing.html %}
{% include components/sections/demo26/lets-talk.html %}
{% include components/sections/demo26/analyze.html %}

</div>
{% include components/footer/footer.html 
  style="minimal-alt"
  bg_color="bg-light"
  container_padding="pt-13 pb-7"
%}
