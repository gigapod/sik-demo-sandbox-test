---
layout: default
title: Sign Up
permalink: /signup2/
custom_color:
custom_font: 
scroll_top_btn:
  enable: true

# Header / Hero Section
hero2:
  title: "Sign Up"
  subtitle: ""
  bg_color: "bg-dark"
  text_color: "text-white"
  breadcrumb:
    - label: "Home"
      url: "#"
    - label: "Sign Up"
      url: ""
      active: true

# Signup Form Section
signup_form:
  title: "Sign up to Sandbox"
  subtitle: "Registration takes less than a minute."
  bg_image: "/assets/img/photos/tm3.jpg"
  form_fields:
    - type: "text"
      id: "loginName"
      label: "Name"
      placeholder: "Name"
    - type: "email"
      id: "loginEmail"
      label: "Email"
      placeholder: "Email"
    - type: "password"
      id: "loginPassword"
      label: "Password"
      placeholder: "Password"
    - type: "password"
      id: "loginPasswordConfirm"
      label: "Confirm Password" 
      placeholder: "Confirm Password"
  button:
    label: "Sign Up"
    url: "#"
  login_link:
    text: "Already have an account?"
    label: "Sign in"
    url: "/signin2"
  social:
    - name: "google"
      icon: "uil uil-google"
    - name: "facebook-f"
      icon: "uil uil-facebook-f"
    - name: "twitter"
      icon: "uil uil-twitter"
---
<div class="content-wrapper">
<header class="wrapper bg-soft-primary">
{% include components/navbar/navbar.html 
    classList="center-nav transparent position-absolute navbar-dark"
    logoBoth=true
    otherClassList="w-100 d-flex ms-auto"
    otherLanguageSelect=true
    otherBtn=true
    otherBtnClassList="btn-sm btn-white rounded-pill"
    otherBtnText="Contact"
    otherBtnLink="/contact.html"
%}
</header>
<!-- /header -->

{% include components/sections/signup/hero2.html %}
{% include components/sections/signup/form.html %}

{% include components/footer/footer.html 
  style="default"
  bg_color="bg-dark"
  text_color="text-inverse"
%}
</div>
