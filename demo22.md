---
layout: default
title: Demo 22
permalink: /demo22/
custom_color: purple
custom_font: urbanist
scroll_top_btn:
  enable: true

# Hero Section
hero:
  subtitle: Hello! We are Sandbox
  title: Grow your business with our marketing solutions
  video_btn:
    enable: true
    url: /assets/media/movie.mp4
  bg_image: /assets/img/photos/bg26.jpg

# Services Section
services:
  title: What We Do?
  subtitle: The full service we are offering is specifically designed to meet your needs.
  service_items:
    - icon: uil uil-monitor
      title: Web Design
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget. Fusce dapibus tellus.
      link_text: Learn More
      link_url: "#"
      color_class: purple
    - icon: uil uil-swatchbook
      title: Graphic Design
      text: Maecenas faucibus mollis interdum. Vivamus sagittis lacus vel augue laoreet. Sed posuere consectetur.
      link_text: Learn More
      link_url: "#"
      color_class: leaf
    - icon: uil uil-presentation-play
      title: 3D Animation
      text: Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus magna scelerisque.
      link_text: Learn More
      link_url: "#"
      color_class: pink

# How It Works Section
how_it_works:
  subtitle: How It Works?
  title: Find out everything about creating a business model.
  image: /assets/img/illustrations/i9.png
  image2x: /assets/img/illustrations/i9@2x.png
  steps:
    - number: 1
      title: Creative Ideas
      text: Nulla vitae elit libero a augue donec id elit non mi porta.
    - number: 2
      title: Magic Touch
      text: Nulla vitae elit libero a augue donec id elit non mi porta.
    - number: 3
      title: Data Analysis
      text: Nulla vitae elit libero a augue donec id elit non mi porta.
    - number: 4
      title: Finalize Product
      text: Nulla vitae elit libero a augue donec id elit non mi porta.

# Why Choose Us Section
why_choose:
  subtitle: Why Choose Us?
  title: We bring solutions to make life easier for our clients.
  image: /assets/img/illustrations/i12.png
  image2x: /assets/img/illustrations/i12@2x.png
  accordion_items:
    - title: Professional Design
      content: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel.
      expanded: true
    - title: Top-Notch Support
      content: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel.
      expanded: false
    - title: Header and Slider Options
      content: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras mattis consectetur purus sit amet fermentum. Praesent commodo cursus magna, vel.
      expanded: false

# Company Facts Section
company_facts:
  title: Company Facts
  subtitle: Save your time and money by choosing our professional team.
  progress_items:
    - title: New Visitors
      value: 75
      color: purple
      text: Maecenas faucibus mollis interdum. Aenean eu leo.
    - title: Social Media
      value: 80
      color: leaf
      text: Maecenas faucibus mollis interdum. Aenean eu leo.
    - title: Referrals
      value: 60
      color: pink
      text: Maecenas faucibus mollis interdum. Aenean eu leo.
    - title: Search Engines
      value: 90
      color: yellow
      text: Maecenas faucibus mollis interdum. Aenean eu leo.

# Projects Section
projects:
  title: Latest Projects
  subtitle: Check out some of our awesome projects with creative ideas and great design.
  

# Pricing Section
pricing:
  title: Our Pricing
  subtitle: We offer great prices, premium products and quality service for your business.
  plans:
    - name: Basic Plan
      monthly_price: 9
      yearly_price: 99
      features:
        - text: <strong>1</strong> Project
        - text: <strong>100K</strong> API Access
        - text: <strong>100MB</strong> Storage
        - text: Weekly <strong>Reports</strong>
        - text: 7/24 <strong>Support</strong>
      button:
        text: Choose Plan
        url: "#"
      is_popular: false
    - name: Premium Plan
      monthly_price: 19
      yearly_price: 199
      features:
        - text: <strong>5</strong> Projects
        - text: <strong>100K</strong> API Access
        - text: <strong>200MB</strong> Storage
        - text: Weekly <strong>Reports</strong>
        - text: 7/24 <strong>Support</strong>
      button:
        text: Choose Plan
        url: "#"
      is_popular: true
    - name: Corporate Plan
      monthly_price: 49
      yearly_price: 499
      features:
        - text: <strong>20</strong> Projects
        - text: <strong>300K</strong> API Access
        - text: <strong>500MB</strong> Storage
        - text: Weekly <strong>Reports</strong>
        - text: 7/24 <strong>Support</strong>
      button:
        text: Choose Plan
        url: "#"
      is_popular: false

# FAQ Section
faq:
  items:
    - question: Can I cancel my subscription?
      answer: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Etiam porta sem malesuada magna mollis euismod maecenas.
    - question: Which payment methods do you accept?
      answer: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Etiam porta sem malesuada magna mollis euismod maecenas.
    - question: How can I manage my Account?
      answer: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Etiam porta sem malesuada magna mollis euismod maecenas.
    - question: Is my credit card information secure?
      answer: Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Etiam porta sem malesuada magna mollis euismod maecenas.

# Call To Action Section
cta:
  title: We are trusted by over 5000+ clients. Join them by using our services and grow your business.
  button:
    text: Join Us
    url: "#"
  bg_image: /assets/img/photos/bg27.jpg
---
<div class="py-md-6">
  <div class="content-wrapper">
    <header class="wrapper">
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

    {% include components/sections/demo22/hero.html %}
    {% include components/sections/demo22/services.html %}
    {% include components/sections/demo22/how-it-works.html %}
    {% include components/sections/demo22/why-choose.html %}
    {% include components/sections/demo22/company-facts.html %}
    {% include components/sections/demo22/projects.html %}
    {% include components/sections/demo22/pricing.html %}
    {% include components/sections/demo22/faq.html %}
    {% include components/sections/demo22/cta.html %}
        
          
     
    {% include components/footer/footer.html 
    style="default"
    bg_color="bg-dark section-frame"
    text_color="text-inverse" 
    cta=false
    %}
  </div>
</div>
