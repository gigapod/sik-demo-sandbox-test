---
layout: default
title: Demo 23
permalink: /demo23/
custom_color: leaf
custom_font: urbanist
scroll_top_btn:
  enable: true

# Hero Section
hero:
  title: I'm Julia Sandbox
  subtitle: couples & wedding photographer
  slides:
    - image: /assets/img/photos/bg28.jpg
      thumbnail: /assets/img/photos/bg28-th.jpg
      thumbnail2x: /assets/img/photos/bg28-th@2x.jpg
    - image: /assets/img/photos/bg29.jpg
      thumbnail: /assets/img/photos/bg29-th.jpg
      thumbnail2x: /assets/img/photos/bg29-th@2x.jpg
    - image: /assets/img/photos/bg30.jpg
      thumbnail: /assets/img/photos/bg30-th.jpg
      thumbnail2x: /assets/img/photos/bg30-th@2x.jpg
    - image: /assets/img/photos/bg31.jpg
      thumbnail: /assets/img/photos/bg31-th.jpg
      thumbnail2x: /assets/img/photos/bg31-th@2x.jpg

# Introduction Section
introduction:
  text: I absolutely love shooting weddings and couples because there are so many feelings to capture.
  categories:
    - title: Wedding
      image: /assets/img/photos/fs1.jpg
      image2x: /assets/img/photos/fs1@2x.jpg
    - title: Couples
      image: /assets/img/photos/fs2.jpg
      image2x: /assets/img/photos/fs2@2x.jpg
    - title: Engagement
      image: /assets/img/photos/fs3.jpg
      image2x: /assets/img/photos/fs3@2x.jpg

# Testimonials Section
testimonials:
  bg_image: /assets/img/photos/bg32.jpg
  

# Video Intro Section
video_intro:
  text: I would like to give you a unique photography and video experience, built to serve you best.
  video_id: 94837904

# Portfolio Section
portfolio:
  title: Some of wonderful love stories I witnessed and had the chance to capture
  portfolio_items:
    - title: Lucy & David
      count: 5
      category: Wedding
      image: /assets/img/photos/fc1.jpg
      image2x: /assets/img/photos/fc1@2x.jpg
    - title: Stacy & Thomas
      count: 8
      category: Wedding
      image: /assets/img/photos/fc2.jpg
      image2x: /assets/img/photos/fc2@2x.jpg
    - title: Katherine & Jack
      count: 7
      category: Couples
      image: /assets/img/photos/fc3.jpg
      image2x: /assets/img/photos/fc3@2x.jpg
    - title: Jolene & William
      count: 9
      category: Wedding
      image: /assets/img/photos/fc4.jpg
      image2x: /assets/img/photos/fc4@2x.jpg
    - title: Jenn & Richard
      count: 6
      category: Engagement
      image: /assets/img/photos/fc5.jpg
      image2x: /assets/img/photos/fc5@2x.jpg
    - title: Gloria & Leo
      count: 8
      category: Wedding
      image: /assets/img/photos/fc6.jpg
      image2x: /assets/img/photos/fc6@2x.jpg
    - title: Grace & Finn
      count: 7
      category: Engagement
      image: /assets/img/photos/fc7.jpg
      image2x: /assets/img/photos/fc7@2x.jpg

# Call to Action Section
cta:
  title: I'm here to capture your moments. Looking for a caring, fun, passionate photographer?
  button:
    text: Contact Me
    url: "#"
  bg_image: /assets/img/photos/bg33.jpg

# About Section
about:
  title: Hi, I'm Julia, a documentary wedding and couples photographer currently working from and based in London.
  text: Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus magna, vel scelerisque nisl consectetur et. Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio. Sed posuere consectetur est at lobortis facilisis in.
  image: /assets/img/photos/about29.jpg
  image2x: /assets/img/photos/about29@2x.jpg
  counters:
    - count: 500K+
      text: Shots Taken
    - count: 500+
      text: Happy Clients
    - count: 25
      text: Awards Won

# Skills Section
skills:
  title: My Skills
  text: Etiam porta sem malesuada magna mollis euismod. Praesent commodo cursus magna vel consectetur purus sit amet fermentum.
  skills_list:
    - name: Photoshop
      value: 100
    - name: Final Cut
      value: 80
    - name: Motion Video
      value: 85
    - name: Manupilation
      value: 75

# Why Choose Me Section
why_choose:
  title: Why Choose Me?
  text: Vestibulum id ligula porta felis euismod semper. Cras mattis consectetur purus sit amet fermentum. Donec ullamcorper nulla non metus auctor fringilla. Nullam id dolor id nibh ultricies. Cras mattis consectetur purus amet fermentum.
  items:
    - text: Aenean eu leo quam pellentesque.
    - text: Nullam quis risus eget urna mollis.
    - text: Donec id elit non mi porta gravida.
    - text: Fusce dapibus tellus ac commodo.
    - text: Cras justo odio dapibus ac facilisis in.

# Process Section
process:
  title: My Process
  steps:
    - number: 1
      title: Collect Ideas
      text: Nulla vitae elit libero pharetra augue dapibus. Praesent commodo cursus.
    - number: 2
      title: Data Analysis
      text: Vivamus sagittis lacus vel augue laoreet. Etiam porta sem malesuada magna.
    - number: 3
      title: Finalize Product
      text: Cras mattis consectetur purus sit amet. Aenean lacinia bibendum nulla sed.

# Blog Section
blog:
  title: Here are the latest posts from my blog that grabbed the most attention.
  
---
<div class="content-wrapper">
  <header class="wrapper bg-soft-primary">
    {% include components/navbar/navbar.html 
        classList="center-nav transparent position-absolute navbar-dark caret-none"
        logoAlt="logo-dark"
        logoLight=true
        logoBoth=true
        otherClassList="w-100 d-flex ms-auto"
        otherSearch=true
        otherInfo=true
    %}
  </header>
  <!-- /header -->

  {% include components/sections/demo23/hero.html %}
  {% include components/sections/demo23/introduction.html %}
  {% include components/sections/demo23/testimonials.html %}
  {% include components/sections/demo23/video-intro.html %}
  {% include components/sections/demo23/portfolio.html %}
  {% include components/sections/demo23/cta.html %}
  {% include components/sections/demo23/about.html %}
  {% include components/sections/demo23/blog.html %}
   
  <!-- /.content-wrapper -->
  
  
</div>
{% include components/footer/footer.html 
  style="default"
  bg_color="bg-dark" 
  text_color="text-inverse"
%}