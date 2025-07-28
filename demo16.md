---
layout: default
title: Demo 16
permalink: /demo16/
custom_color: pink
custom_font: thicccboi
scroll_top_btn:
  enable: true


# Hero Section
hero:
  image: /assets/img/photos/about17.webp
  image2x: /assets/img/photos/about17@2x.webp
  card:
    icon: /assets/img/icons/lineal/check.svg
    count: 250+
    text: Projects Done
  title: I'm User Interface Designer & Developer.
  subtitle: Hello! I'm Julia, a freelance user interface designer & developer based in London. I'm very passionate about the work that I do.
  buttons:
    - label: See My Works
      url: "#"
      class: btn btn-lg btn-primary rounded-pill me-2
    - label: Contact Me
      url: "#"
      class: btn btn-lg btn-outline-primary rounded-pill

# Skills Section
skills:
  title: What I Do?
  text: Duis mollis est commodo luctus nisi erat porttitor ligula, eget lacinia odio sem nec elit. Nullam quis risus eget urna mollis ornare vel. Nulla vitae elit libero, a pharetra augue. Praesent commodo cursus magna, vel scelerisque nisl.
  progress_items:
    - name: Web Design
      value: 100
      class: soft-violet
    - name: Mobile Design
      value: 80
      class: soft-blue
    - name: Development
      value: 85
      class: soft-leaf
    - name: SEO
      value: 90
      class: soft-pink
  service_items:
    - icon: /assets/img/icons/lineal/browser.svg
      color: violet
      title: Web Design
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus. Cras justo cum sociis natoque magnis.
    - icon: /assets/img/icons/lineal/smartphone.svg
      color: blue
      title: Mobile Design
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus. Cras justo cum sociis natoque magnis.
    - icon: /assets/img/icons/lineal/settings-3.svg
      color: leaf
      title: Development
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus. Cras justo cum sociis natoque magnis.
    - icon: /assets/img/icons/lineal/search-2.svg
      color: pink
      title: SEO
      text: Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus. Cras justo cum sociis natoque magnis.

# Projects Section
projects:
  title: Latest Projects
  text: Check out some of my latest projects with creative ideas.
  button:
    label: See All Projects
    url: "/projects-tiles"
  
# Contact Section
contact:
  icon: /assets/img/icons/lineal/email.svg
  title: If you like what you see, let's work together.
  text: I bring rapid solutions to make the life of my clients easier. Have any questions? Reach out to me from this contact form and I will get back to you shortly.
---
<div class="content-wrapper">
<header class="wrapper bg-gray">
{% include components/navbar/navbar.html 
    classList="fancy navbar-light navbar-bg-light"
    fancy=true
    logoAlt="logo-dark"
    otherClassList="w-100 d-flex ms-auto"
    otherSocial=true
%}
</header>
<!-- /header -->

{% include components/sections/demo16/hero.html %}
{% include components/sections/demo16/skills.html %}
{% include components/sections/demo16/projects.html %}
{% include components/sections/demo16/contact.html 
  form=true
%}
</div>
{% include components/footer/footer.html 
  style="minimal" 
  container_padding="pt-3 pt-md-4 pb-7"
%}
