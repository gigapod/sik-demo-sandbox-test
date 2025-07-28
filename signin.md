---
layout: default
title: Sign In
permalink: /signin/
custom_color:
custom_font: 
scroll_top_btn:
  enable: true

# Header / Hero Section
hero:
  title: "Sign In"
  bg_image: "/assets/img/photos/bg18.png"
  bg_overlay: "bg-overlay-light-600"
  breadcrumb:
    - label: "Home"
      url: "#"
    - label: "Sign In"
      url: ""

# Sign In Form Section
signin_form:
  title: "Welcome Back"
  subtitle: "Fill your email and password to sign in."
  form_fields:
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
    url: "#"
  forgot_password:
    label: "Forgot Password?"
    url: "#"
  signup:
    label: "Don't have an account? Sign up"
    url: "/signup/"
  social_login:
    enabled: true
    options:
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
    classList= "center-nav transparent position-absolute navbar-light"
    otherClassList= "w-100 d-flex ms-auto"
    otherLanguageSelect= true
    otherBtn= true
    otherBtnClassList= "btn-sm btn-primary rounded-pill"
    otherBtnText= "Contact"
    otherBtnLink= "/contact"
%}
</header>
<!-- /header -->

{% include components/sections/signin/hero.html %}
{% include components/sections/signin/signin-form.html %}

{% include components/footer/footer.html 
  style= "default"
  bg_color= "bg-dark"
  text_color= "text-inverse"
%}
</div>
