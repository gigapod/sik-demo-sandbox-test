---
layout: default
title: Join Our Team
permalink: /career2/
custom_color:
custom_font: 
scroll_top_btn:
  enable: true

# Header / Hero Section
hero:
  title: "Join Our Team"
  subtitle: "Join our team to help shape the future of development."
  bg_color: "bg-soft-primary"
  button:
    label: "Explore Positions"
    url: "#"

# Benefits Section
benefits:
  items:
    - icon: "target"
      title: "Career Growth"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus cras justo."
    - icon: "videocall"
      title: "Work From Anywhere"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus cras justo."
    - icon: "wallet"
      title: "Smart Salary"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus cras justo."
    - icon: "alarm"
      title: "Flexible Hours"
      text: "Nulla vitae elit libero, a pharetra augue. Donec id elit non mi porta gravida at eget metus cras justo."

# About Us Section
about_us:
  title: "What Makes Us Different?"
  subtitle: "We bring solutions to make life easier for our customers."
  text: "Etiam porta sem malesuada magna mollis euismod. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Nulla vitae elit libero, a pharetra augue. Etiam porta sem malesuada magna mollis euismod. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Maecenas sed."
  features:
    - icon: "share"
      title: "Our Mission"
      text: "Curabitur blandit lacus porttitor ridiculus mus."
    - icon: "partnership"
      title: "Our Values"
      text: "Curabitur blandit lacus porttitor ridiculus mus."
  images:
    - src: /assets/img/photos/g8.jpg
      src2x: /assets/img/photos/g8@2x.jpg
      class: "col-12"
    - src: /assets/img/photos/g9.jpg
      src2x: /assets/img/photos/g9@2x.jpg
      class: "col-md-6"
    - src: /assets/img/photos/g10.jpg
      src2x: /assets/img/photos/g10@2x.jpg
      class: "col-md-6"

# Jobs Section
jobs:
  title: "Job Positions"
  subtitle: "We're always searching for amazing people to join our team. Take a look at our current openings."
  filters:
    - name: "Position"
      options:
        - label: "Business"
          value: "position1"
        - label: "Design" 
          value: "position2"
        - label: "Development"
          value: "position3"
        - label: "Engineering"
          value: "position4"
        - label: "Finance"
          value: "position5"
        - label: "Marketing"
          value: "position6"
    - name: "Type"
      options:
        - label: "Full-time"
          value: "type1"
        - label: "Part-time"
          value: "type3"
        - label: "Remote"
          value: "type4"
    - name: "Location"
      options:
        - label: "Chicago, US"
          value: "location1"
        - label: "Michigan, US"
          value: "location3"
        - label: "New York, US"
          value: "location2"
        - label: "Los Angles, US"
          value: "location4"
        - label: "Moscow, Russia"
          value: "location5"
        - label: "Sydney, Australia"
          value: "location6"
        - label: "Birmingham, UK"
          value: "location7"
        - label: "Manchester, UK"
          value: "location8"
        - label: "Beijing, China"
          value: "location9"
  categories:
    - name: "Design"
      positions:
        - title: "Senior Graphic Designer"
          avatar: "GD"
          avatar_bg: "bg-red"
          type: "Full time"
          location: "San Francisco, US"
        - title: "UI/UX Designer"
          avatar: "UX"
          avatar_bg: "bg-green"
          type: "Remote"
          location: "Anywhere"
        - title: "Multimedia Artist & Animator"
          avatar: "AN"
          avatar_bg: "bg-yellow"
          type: "Full time"
          location: "Birmingham, UK"
    - name: "Development"
      positions:
        - title: "Front End Developer"
          avatar: "FE"
          avatar_bg: "bg-purple"
          type: "Part time"
          location: "Sydney, AU"
        - title: "Mobile Developer"
          avatar: "MD"
          avatar_bg: "bg-orange"
          type: "Full-time"
          location: "San Francisco, US"
        - title: ".NET Developer"
          avatar: "NT"
          avatar_bg: "bg-pink"
          type: "Full time"
          location: "Manchester, UK"

# Contact Section
contact:
  title: "Can't find the right position?"
  subtitle: "We are a community with 5000+ team members. Join and build the future with us."
  button:
    label: "Contact Us"
    url: "#"
---
<div class="content-wrapper">
<header class="wrapper bg-soft-primary">
{% include components/navbar/navbar.html 
    classList="center-nav transparent navbar-light"
    otherClassList="w-100 d-flex ms-auto"
    otherLanguageSelect=true
    otherBtn=true
    otherBtnClassList="btn-sm btn-primary rounded-pill"
    otherBtnText="Contact"
    otherBtnLink="/contact"
%}
</header>
<!-- /header -->

{% include components/sections/career2/hero.html %}
{% include components/sections/career2/benefits.html %}
{% include components/sections/career2/about-us.html %}
{% include components/sections/career2/jobs.html %}
{% include components/sections/career2/contact.html %}

{% include components/footer/footer.html 
  style="default"
  bg_color="bg-dark"
  text_color="text-inverse"
%}
</div>
