---
layout: default
title: Demo 31
permalink: /demo31/
custom_color: primary
custom_font: space
scroll_top_btn:
  enable: true

# Hero Section
hero:
  bg_class: "wrapper"
  title: "We bring rapid solutions for your <span class=\"underline-3 style-1 primary\"><em>business</em></span>"
  title_class: "display-1 ls-sm fs-64 mb-4 px-md-8 px-lg-0"
  text: "We are creative company that values quality and focuses on establishing long-term relationships with customers."
  text_class: "lead fs-24 lh-sm mb-7"
  button:
    label: "See Projects"
    url: "#"
    class: "btn btn-lg btn-primary rounded mb-10 mb-xxl-5"
  image: "/assets/img/illustrations/i28.png"
  image2x: "/assets/img/illustrations/i28@2x.png"
  divider: true
  divider_color: "text-soft-primary"

# Trusted Clients Section
trusted_clients:
  title: "Trusted by over 5000 clients"
  title_class: "fs-16 text-uppercase text-muted mb-8 text-center"
 

# Services Section
services:
  title: "Our Services"
  title_class: "fs-16 text-uppercase text-muted mb-3"
  main_title: "The service we offer is <span class=\"underline-3 style-1 primary\"><em>designed</em></span> to meet your business needs."
  main_title_class: "display-2 ls-sm px-xxl-10"
  service_items:
    - image: "/assets/img/illustrations/i29.png"
      image2x: "/assets/img/illustrations/i29@2x.png"
      icon: "/assets/img/icons/solid/like.svg"
      icon_class: "bg-pale-primary"
      icon_text_class: "text-primary"
      title: "Social Media Marketing"
      text: "Maecenas faucibus mollis interdum sed posuere consectetur est at lobortis. Scelerisque id ligula porta felis euismod semper. Fusce dapibus tellus."
      features:
        - text: "Aenean eu leo quam. Pellentesque ornare."
        - text: "Nullam quis risus eget urna mollis ornare."
        - text: "Fusce dapibus, tellus ac cursus commodo."
      button:
        label: "Learn More"
        url: "#"
        class: "more hover link-primary"
    - image: "/assets/img/illustrations/i30.png"
      image2x: "/assets/img/illustrations/i30@2x.png"
      icon: "/assets/img/icons/solid/layout-2.svg"
      icon_class: "bg-pale-green"
      icon_text_class: "text-green"
      title: "Web Design & Development"
      text: "Maecenas faucibus mollis interdum sed posuere consectetur est at lobortis. Scelerisque id ligula porta felis euismod semper. Fusce dapibus tellus."
      features:
        - text: "Aenean eu leo quam. Pellentesque ornare."
        - text: "Nullam quis risus eget urna mollis ornare."
        - text: "Fusce dapibus, tellus ac cursus commodo."
      button:
        label: "Learn More"
        url: "#"
        class: "more hover link-green"
      reverse: true
    - image: "/assets/img/illustrations/i31.png"
      image2x: "/assets/img/illustrations/i31@2x.png"
      icon: "/assets/img/icons/solid/bullhorn.svg"
      icon_class: "bg-pale-fuchsia"
      icon_text_class: "text-fuchsia"
      title: "Content Marketing Services"
      text: "Maecenas faucibus mollis interdum sed posuere consectetur est at lobortis. Scelerisque id ligula porta felis euismod semper. Fusce dapibus tellus."
      features:
        - text: "Aenean eu leo quam. Pellentesque ornare."
        - text: "Nullam quis risus eget urna mollis ornare."
        - text: "Fusce dapibus, tellus ac cursus commodo."
      button:
        label: "Learn More"
        url: "#"
        class: "more hover link-fuchsia"

# Testimonials Section
testimonials:
  bg_class: "card bg-soft-primary rounded-4"
  title: "Happy Customers"
  title_class: "fs-16 text-uppercase text-muted mb-3"
  main_title: "Don't take our word for it. See what our <span class=\"underline-3 style-1 primary\"><em>customers</em></span> are saying about us."
  main_title_class: "display-2 ls-sm mb-10 px-xxl-10"
  image: "/assets/img/photos/about13.jpg"
  image2x: "/assets/img/photos/about13@2x.jpg"
  

# Projects Section
projects:
  title: "Latest Projects"
  title_class: "fs-16 text-uppercase text-muted mb-3"
  main_title: "Check out some of our <span class=\"underline-3 style-1 primary\"><em>awesome</em></span> projects with creative ideas and great design."
  main_title_class: "display-2 ls-sm"
  

# Join Community Section
join_community:
  title: "Join Our Community"
  title_class: "fs-16 text-uppercase text-muted mb-3"
  main_title: "We are <span class=\"underline-3 style-1 primary\"><em>trusted</em></span> by over 50000+ clients. Join them now and grow your business."
  main_title_class: "display-2 ls-sm"
  counters:
    - count: "1000+"
      text: "Completed Projects"
    - count: "50K+"
      text: "Happy Customers"
    - count: "4x"
      text: "Revenue Growth"
  image: "/assets/img/illustrations/i32.png"
  image2x: "/assets/img/illustrations/i32@2x.png"
  divider: true
  divider_color: "text-soft-primary"

# Footer
footer:
  bg_class: "bg-soft-primary"
---
<div class="content-wrapper">
<header class="wrapper bg-light">

  {% include components/navbar/navbar.html 
    topInfo=true
    wrapperClass="bg-light"
    classList="center-nav transparent navbar-light"
    otherClassList="w-100 d-flex ms-auto"
    otherLanguageSelect=true
    otherBtn=true
    otherBtnClassList="btn btn-sm btn-primary rounded-pill"
    otherBtnText="Contact"
    otherBtnLink="/contact/"
%}

</header>
<!-- /header -->

{% include components/sections/demo31/hero.html %}
{% include components/sections/demo31/trusted-clients.html %}
{% include components/sections/demo31/services.html %}
{% include components/sections/demo31/testimonials.html %}
{% include components/sections/demo31/projects.html %}
{% include components/sections/demo31/join-community.html %}

</div>
{% include components/footer/footer.html 
  style="default"
  bg_color="bg-soft-primary"
  text_color="text-dark"
  widget_title_class="text-dark"
  cta=false
%}
