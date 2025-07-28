---
layout: default
title: Demo 25
permalink: /demo25/
custom_color: pink
custom_font: urbanist
scroll_top_btn:
  enable: true

author: Jane Smith

# Header Settings
navbar:
  classList: "center-nav navbar-light navbar-bg-light"
  logoAlt: "logo-dark"
  otherClassList: "w-100 d-flex ms-auto"
  otherSocial: true

# Hero Slider Section
hero_slider:
  enable: true
  

# Intro Section
intro:
  title: Hello! I'm Caitlyn. Welcome to my blog. Here on this blog you will be able to find travel diary with traveling tips.

# Categories Section
categories:
  items:
    - title: About Me
      image: /assets/img/photos/f1.jpg
      link: "#"
      details: Read Details
    - title: Destinations
      image: /assets/img/photos/f2.jpg
      link: "#"
      details: See Destinations
    - title: Instagram
      image: /assets/img/photos/f3.jpg
      link: "#"
      details: Follow Me

# Blog Posts
blog_posts:
  
# Sidebar
sidebar:
  
---
<div class="content-wrapper">
<header class="wrapper bg-gray">
{% include components/navbar/navbar.html 
    classList=page.navbar.classList
    logoAlt=page.navbar.logoAlt
    otherClassList=page.navbar.otherClassList
    otherSocial=page.navbar.otherSocial
%}
</header>
<!-- /header -->

{% include components/sections/demo25/hero-slider.html %}
{% include components/sections/demo25/intro.html %}
{% include components/sections/demo25/categories.html %}
{% include components/sections/demo25/blog-posts.html %}

</div>
{% include components/footer/footer.html 
  style="blog" 
  container_padding="py-13 py-md-15"
  bg_color="bg-dark"
  text_color="text-inverse"
%}
