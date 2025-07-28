---
layout: default
title: Sign In
permalink: /signin2/
custom_color:
custom_font: 
scroll_top_btn:
  enable: true

# Header / Hero Section
hero:
  title: "Sign In"
  bg_color: "bg-dark"
  text_color: "text-white"
  breadcrumb:
    - label: "Home"
      url: "#"
    - label: "Sign In"
      url: ""
      active: true

# Sign-in Form Section
signin_form:
  title: "Welcome Back"
  subtitle: "Fill your email and password to sign in."
  image: 
    src: "/assets/img/photos/tm3.jpg"
    position: "left"
  form:
    fields:
      - type: "email"
        id: "loginEmail"
        placeholder: "Email"
        label: "Email"
      - type: "password"
        id: "loginPassword"
        placeholder: "Password"
        label: "Password"
    button:
      label: "Sign In"
      class: "btn-primary rounded-pill btn-login w-100 mb-2"
  links:
    - label: "Forgot Password?"
      url: "#"
    - label: "Don't have an account? Sign up"
      url: "/signup2/"
  social:
    enabled: true
    platforms:
      - name: "google"
        icon: "uil-google"
      - name: "facebook-f"
        icon: "uil-facebook-f"
      - name: "twitter"
        icon: "uil-twitter"
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
    otherBtnLink="/contact"
%}
</header>
<!-- /header -->

{% include components/sections/signin/hero.html %}
{% include components/sections/signin/form.html %}

{% include components/footer/footer.html 
  style="default"
  bg_color="bg-dark"
  text_color="text-inverse"
%}
</div>
