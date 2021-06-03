---
layout: home
---

<header>
  <div class="logo-container">
    <svg class="wmrug-logo" viewBox="0 0 16 18" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M6 8H10L12 10L10 18H6L4 10L6 8Z" fill="#720F0F"/>
      <path d="M6 8L2 6L0 8L4 10L6 8Z" fill="#ECC5C5"/>
      <path d="M14 6L10 8L12 10L16 8L14 6Z" fill="#ECC5C5"/>
      <path d="M2 2V6L0 8V6L2 2Z" fill="#FBDFDF"/>
      <path d="M14 6V2L16 6V8L14 6Z" fill="#FBDFDF"/>
      <path d="M4 10L0 8L6 18L4 10Z" fill="#C93636"/>
      <path d="M12 10L16 8L10 18L12 10Z" fill="#C93636"/>
      <path d="M2 2V6L6 8H10L14 6V2L10 0H6L2 2Z" fill="#C44343"/>
    </svg>
  </div>

  <h1 class="main-title">West Midlands<br>Ruby User Group</h1>

  <p class="tagline">
    Promoting the <a href="https://www.ruby-lang.org/en/">Ruby</a> programming language in the West Midlands and beyond.
  </p>
</header>

<div class="cta">
  <div class="cta-link"><a href="https://www.meetup.com/West-Midlands-Ruby-User-Group-WMRUG/">JOIN US</a></div>
  <div class="cta-subtitle"><small>(almost)</small> every third Wednesday!</div>
</div>

<section class="prose">
  <h2>Recent Events</h2>

  {% for item in site.data.recentevents %}
    <h3>
      {% if item.link %}
      <a href="{{ item.link }}">{{ item.date }} - {{ item.name }}</a>
      {% else %}
      {{ item.date }} - {{ item.name }}
      {% endif %}
    </h3>

    <p>
      {{ item.description }}
    </p>
  {% endfor %}
</section>
