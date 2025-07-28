---
layout: default
title: Contact
permalink: /contact2/
custom_color:
custom_font: 
scroll_top_btn:
  enable: true

# Header / Hero Section
hero:
  title: "Get in Touch"
  bg_color: "bg-soft-primary"
  breadcrumb:
    enable: true
    items:
      - label: "Home"
        url: "#"
        active: false
      - label: "Contact"
        active: true

# Contact Info Section
contact_info:
  title: "Convinced yet? Let's make something great together."
  image1: /assets/img/photos/g5.jpg
  image1_2x: /assets/img/photos/g5@2x.jpg
  image2: /assets/img/photos/g6.jpg
  image2_2x: /assets/img/photos/g6@2x.jpg
  counter:
    value: "5000+"
    label: "Satisfied Customers"
  items:
    - icon: "location-pin-alt"
      title: "Address"
      text: "Moonshine St. 14/05 Light City, <br>London, United Kingdom"
    - icon: "phone-volume"
      title: "Phone"
      text: "00 (123) 456 78 90"
    - icon: "envelope"
      title: "E-mail"
      text: "<a href='mailto:sandbox@email.com' class='link-body'>sandbox@email.com</a>"

# Contact Form Section
contact_form:
  title: "Drop Us a Line"
  subtitle: "Reach out to us from our contact form and we will get back to you shortly."
  note: "<strong>*</strong> These fields are required."
  button:
    label: "Send message"
    class: "btn btn-primary rounded-pill btn-send mb-3"
  fields:
    - id: "form_name"
      name: "name"
      type: "text"
      label: "First Name *"
      placeholder: "Jane"
      required: true
      col: "col-md-6"
    - id: "form_lastname"
      name: "surname"
      type: "text"
      label: "Last Name *"
      placeholder: "Doe"
      required: true
      col: "col-md-6"
    - id: "form_email"
      name: "email"
      type: "email"
      label: "Email *"
      placeholder: "jane.doe@example.com"
      required: true
      col: "col-md-6"
    - id: "form-select"
      name: "department"
      type: "select"
      label: "Select a department"
      required: true
      col: "col-md-6"
      options:
        - label: "Sales"
          value: "Sales"
        - label: "Marketing"
          value: "Marketing"
        - label: "Customer Support"
          value: "Customer Support"
    - id: "form_message"
      name: "message"
      type: "textarea"
      label: "Message *"
      placeholder: "Your message"
      required: true
      height: "150px"
      col: "col-12"
---
<div class="content-wrapper">
<header class="wrapper bg-soft-primary">
{% include components/navbar/navbar.html 
    classList="center-nav transparent navbar-light"
    otherClassList="w-100 d-flex ms-auto"
    otherLanguageSelect=true
    otherBtn=true
    otherBtnClassList="btn btn-sm btn-primary rounded-pill"
    otherBtnText="Contact"
    otherBtnLink="/contact.html"
%}
</header>
<!-- /header -->

{% include components/sections/contact2/hero.html %}

<section class="wrapper bg-light angled upper-end">
  <div class="container py-14 py-md-16">
    {% include components/sections/contact2/contact-info.html %}
    {% include components/sections/contact2/contact-form.html %}
  </div>
  <!-- /.container -->
</section>
<!-- /section -->

{% include components/footer/footer.html 
  style="default"
  bg_color="bg-dark"
  text_color="text-inverse"
%}
</div>
