---
layout: default
title: Multimedia Artist & Animator
permalink: /career-job/
custom_color:
custom_font: 
scroll_top_btn:
  enable: true

# Job Details
job:
  title: "Multimedia Artist & Animator"
  meta:
    - icon: "uil uil-clock"
      text: "Full time"
    - icon: "uil uil-location-arrow"
      text: "Manchester, UK" 
    - icon: "uil uil-building"
      text: "Design Department"
  apply_button:
    email: "apply@email.com"
    label: "Apply Now"

# Job Description
job_description:
  title: "Job Description"
  content: |
    Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Cras mattis consectetur purus sit amet fermentum. Aenean lacinia bibendum nulla sed consectetur. Curabitur blandit tempus porttitor. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Nullam quis risus eget porta ac consectetur vestibulum.

    Donec sed odio dui consectetur adipiscing elit. Etiam adipiscing tincidunt elit, eu convallis felis suscipit ut. Phasellus rhoncus tincidunt auctor. Nullam eu sagittis mauris. Donec non dolor ac elit aliquam tincidunt at at sapien. Aenean tortor libero, condimentum ac laoreet vitae, varius tempor nisi. Duis non arcu vel lectus urna mollis ornare vel eu leo.

# Responsibilities
responsibilities:
  title: "Responsibilities"
  intro: "Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus magna, vel scelerisque nisl consectetur et."
  items:
    - "Aenean eu leo quam ornare curabitur blandit tempus."
    - "Nullam quis risus eget urna mollis ornare donec elit."
    - "Etiam porta sem malesuada magna mollis euismod."
    - "Fermentum massa vivamus faucibus amet euismod."

# Requirements
requirements:
  title: "Requirements"
  intro: "Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Praesent commodo cursus magna, vel scelerisque nisl consectetur et."
  items:
    - "Aenean eu leo quam ornare curabitur blandit tempus."
    - "Nullam quis risus eget urna mollis ornare donec elit."
    - "Etiam porta sem malesuada magna mollis euismod."
    - "Fermentum massa vivamus faucibus amet euismod."

# More Jobs Section
more_jobs:
  title: "More Job Openings"
  button:
    label: "Explore Positions"
    url: "#"
  positions:
    - title: "Senior Graphic Designer"
      avatar: "SD"
      avatar_bg: "bg-red"
      type: "Full Time"
      type_bg: "bg-pale-blue text-blue"
      location: "San Francisco, US"
    - title: "UI/UX Designer"
      avatar: "UX"
      avatar_bg: "bg-green"
      type: "Remote"
      type_bg: "bg-pale-aqua text-aqua"
      location: "Anywhere"
    - title: "Multimedia Artist & Animator"
      avatar: "AN"
      avatar_bg: "bg-yellow"
      type: "Full Time"
      type_bg: "bg-pale-blue text-blue"
      location: "Birmingham, UK"
    - title: "Front End Developer"
      avatar: "FD"
      avatar_bg: "bg-purple"
      type: "Part Time"
      type_bg: "bg-pale-violet text-violet"
      location: "Sydney, AU"
    - title: "Mobile Developer"
      avatar: "MD"
      avatar_bg: "bg-orange"
      type: "Full Time"
      type_bg: "bg-pale-blue text-blue"
      location: "San Francisco, US"
    - title: ".NET Developer"
      avatar: "ND"
      avatar_bg: "bg-pink"
      type: "Full Time"
      type_bg: "bg-pale-blue text-blue"
      location: "Manchester, UK"
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

{% include components/sections/career-job/hero.html %}
{% include components/sections/career-job/job-content.html %}
{% include components/sections/career-job/more-jobs.html %}

{% include components/footer/footer.html 
  style="default"
  bg_color="bg-dark"
  text_color="text-inverse"
%}
</div>
