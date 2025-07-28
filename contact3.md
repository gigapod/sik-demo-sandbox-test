---
layout: default
title: Contact
permalink: /contact3/
custom_color:
custom_font: 
scroll_top_btn:
  enable: true

# Header / Hero Section
hero:
  title: "Get in Touch"
  subtitle: "Have any questions? Reach out to us from our contact form and we will get back to you shortly."
  bg_color: "bg-dark"
  text_color: "text-white"

# Contact Card Section
contact_card:
  image: "/assets/img/photos/tm1.jpg"
  title: "Let's Talk"
  lead_text: "Let's make something great together. We are trusted by over 5000+ clients. Join them by using our services and grow your business."
  text: "Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Maecenas faucibus mollis interdum. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus."
  button:
    label: "Join Us"
    url: "#"

# Contact Form Section
contact_form:
  title: ""
  subtitle: ""
  departments:
    - "Sales"
    - "Marketing"
    - "Customer Support"

# Contact Info
contact_info:
  address:
    icon: "location-pin-alt"
    title: "Address"
    text: "Moonshine St. 14/05 Light City, London, United Kingdom"
  phone:
    icon: "phone-volume"
    title: "Phone"
    lines:
      - "00 (123) 456 78 90"
      - "00 (987) 654 32 10"
  email:
    icon: "envelope"
    title: "E-mail"
    addresses:
      - address: "sandbox@email.com"
        url: "mailto:sandbox@email.com"
      - address: "help@sandbox.com"
        url: "mailto:help@sandbox.com"

# Map Section
map:
  embed_url: "https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d25387.23478654725!2d-122.06115399490332!3d37.309248660190086!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x808fb4571bd377ab%3A0x394d3fe1a3e178b4!2sCupertino%2C%20CA%2C%20USA!5e0!3m2!1sen!2str!4v1645437305701!5m2!1sen!2str"
  height: 500
---
<div class="content-wrapper">
<header class="wrapper bg-soft-primary">
{% include components/navbar/navbar.html 
    classList="center-nav transparent position-absolute navbar-dark"
    logoBoth=true
    otherClassList="w-100 d-flex ms-auto"
    otherLanguageSelect=true
    otherBtn=true
    otherBtnClassList="btn btn-sm btn-white rounded-pill"
    otherBtnText="Contact"
    otherBtnLink="/contact.html"
%}
</header>
<!-- /header -->

{% include components/sections/contact3/hero.html %}
{% include components/sections/contact3/contact-card.html %}
{% include components/sections/contact3/contact-form.html %}
{% include components/sections/contact3/map.html %}

{% include components/footer/footer.html 
  style="default"
  bg_color="bg-dark"
  text_color="text-inverse"
%}
</div>
