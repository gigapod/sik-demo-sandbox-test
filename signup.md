---
layout: default
title: Sign Up
permalink: /signup/
custom_color:
custom_font: 
scroll_top_btn:
  enable: true

# Header / Hero Section
hero:
  title: "Sign Up"
  subtitle: ""
  bg_image: "/assets/img/photos/bg18.png"
  bg_overlay: "bg-overlay-light-600"
  breadcrumb:
    - label: "Home"
      url: "#"
    - label: "Sign Up"
      url: ""

# Signup Form Section
signup_form:
  title: "Sign up to Sandbox"
  subtitle: "Registration takes less than a minute."
  form_fields:
    - id: "loginName"
      type: "text"
      placeholder: "Name"
      label: "Name"
    - id: "loginEmail"
      type: "email"
      placeholder: "Email"
      label: "Email"
    - id: "loginPassword"
      type: "password"
      placeholder: "Password"
      label: "Password"
    - id: "loginPasswordConfirm"
      type: "password"
      placeholder: "Confirm Password"
      label: "Confirm Password"
  button:
    label: "Sign Up"
    url: "#"
  login_text: "Already have an account?"
  login_link: "/signin"
  login_label: "Sign in"
  social_divider: "or"
  social_buttons:
    - platform: "google"
      icon: "uil uil-google"
      url: "#"
    - platform: "facebook-f"
      icon: "uil uil-facebook-f"
      url: "#"
    - platform: "twitter"
      icon: "uil uil-twitter"
      url: "#"
---
<div class="content-wrapper">
<header class="wrapper bg-soft-primary">
{% include components/navbar/navbar.html 
    classList= "center-nav transparent navbar-light"
    otherClassList= "w-100 d-flex ms-auto"
    otherLanguageSelect= true
    otherBtn= true
    otherBtnClassList= "btn-sm btn-primary rounded-pill"
    otherBtnText= "Contact"
    otherBtnLink= "/contact"
%}
</header>
<!-- /header -->

{% include components/sections/signup/hero.html %}
{% include components/sections/signup/signup-form.html %}

{% include components/footer/footer.html 
  style= "default"
  bg_color= "bg-dark"
  text_color= "text-inverse"
%}
</div>
