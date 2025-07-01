---
layout: single
title: "Canva Portfolio"
permalink: /canva/
author_profile: true
---

Welcome to my Canva design portfolio! Below are collections of my visual work, organized by project or topic.

---

## 📁 Edmonton Global

A collection of designs that I created for Edmonton Global (their social media and website) during my internship.

<div style="text-align: center; margin: 1em 0;">
  <img id="edmonton-slide" src="" alt="Edmonton Design" style="max-height: 400px; width: auto; border: 1px solid #ddd; border-radius: 8px;">
</div>

<div style="display: flex; justify-content: center; align-items: center; gap: 1rem; margin: 1em 0;">
  <button onclick="edmontonCarouselPrev()" class="carousel-btn" aria-label="Previous" style="padding: 0.3em 1em; font-size: 0.9em;">
    <span style="font-size: 1.2em; display: inline-block; transform: rotate(-20deg); color: #7b2ff2;">&#8592;</span>
    <span style="font-family: 'Brush Script MT', cursive; font-size: 1em; color: #7b2ff2; margin-left: 0.2em;">Prev</span>
  </button>

  <button onclick="edmontonCarouselNext()" class="carousel-btn" aria-label="Next" style="padding: 0.3em 1em; font-size: 0.9em;">
    <span style="font-family: 'Brush Script MT', cursive; font-size: 1em; color: #f357a8; margin-right: 0.2em;">Next</span>
    <span style="font-size: 1.2em; display: inline-block; transform: rotate(20deg); color: #f357a8;">&#8594;</span>
  </button>
</div>

<script>
  const edmontonImages = [
    {% assign folder = "assets/Canva/Edmonton Global" %}
    {% for file in site.static_files %}
      {% if file.path contains folder %}
        {% if file.extname == ".png" or file.extname == ".jpg" or file.extname == ".jpeg" %}
          "{{ site.baseurl }}{{ file.path }}",
        {% endif %}
      {% endif %}
    {% endfor %}
  ];

  let edmontonIndex = 0;

  function showEdmontonSlide(index) {
    const img = document.getElementById('edmonton-slide');
    if (img && edmontonImages.length > 0) {
      img.src = edmontonImages[index];
    }
  }

  function edmontonCarouselPrev() {
    edmontonIndex = (edmontonIndex - 1 + edmontonImages.length) % edmontonImages.length;
    showEdmontonSlide(edmontonIndex);
  }

  function edmontonCarouselNext() {
    edmontonIndex = (edmontonIndex + 1) % edmontonImages.length;
    showEdmontonSlide(edmontonIndex);
  }

  // Initialize on page load
  document.addEventListener("DOMContentLoaded", () => {
    showEdmontonSlide(edmontonIndex);
  });
</script>

---

## 📄 DUSS Year-in-Review

<a href="{{ site.baseurl }}/assets/Canva/duss_year-in-review.pdf" target="_blank" rel="noopener">Download the PDF report</a>

---

## 📁 Media Studies

_Designs created for my Media Studies courses._

<div id="media-studies-carousel" style="max-width: 800px; margin: 0 auto; text-align: center;">
   <img id="media-carousel-image" src="{{ site.baseurl }}/assets/Canva/Media Studies/Collage_C LIT 352.png" width="300" style="border-radius: 18px; box-shadow: 0 6px 24px rgba(0,0,0,0.18); transition: box-shadow 0.3s, transform 0.3s;" />
   <div style="margin-top: 1rem; display: flex; justify-content: center; gap: 1.5em;">
      <button onclick="mediaCarouselPrev()" class="carousel-btn" aria-label="Previous" style="padding: 0.3em 1em; font-size: 0.9em;">
         <span style="font-size: 1.2em; display: inline-block; transform: rotate(-20deg); color: #7b2ff2;">&#8592;</span>
         <span style="font-family: 'Brush Script MT', cursive; font-size: 1em; color: #7b2ff2; margin-left: 0.2em;">Prev</span>
      </button>
      <button onclick="mediaCarouselNext()" class="carousel-btn" aria-label="Next" style="padding: 0.3em 1em; font-size: 0.9em;">
         <span style="font-family: 'Brush Script MT', cursive; font-size: 1em; color: #f357a8; margin-right: 0.2em;">Next</span>
         <span style="font-size: 1.2em; display: inline-block; transform: rotate(20deg); color: #f357a8;">&#8594;</span>
      </button>
   </div>
</div>
<script>
const mediaCarouselImages = [
    {% assign folder = "assets/Canva/Media Studies/Learn Ukrainian_MST 210" %}
    {% for file in site.static_files %}
      {% if file.path contains folder %}
        {% if file.extname == ".png" or file.extname == ".jpg" or file.extname == ".jpeg" %}
          "{{ site.baseurl }}{{ file.path }}",
        {% endif %}
      {% endif %}
    {% endfor %},
      {% assign folder = "assets/Canva/Media Studies/" %}
    {% for file in site.static_files %}
      {% if file.path contains folder %}
        {% if file.extname == ".png" or file.extname == ".jpg" or file.extname == ".jpeg" %}
          "{{ site.baseurl }}{{ file.path }}",
        {% endif %}
      {% endif %}
    {% endfor %}
   ];
   let mediaCarouselIndex = 0;
   function updateMediaCarousel() {
      document.getElementById('media-carousel-image').src = mediaCarouselImages[mediaCarouselIndex];
   }
   function mediaCarouselPrev() {
      mediaCarouselIndex = (mediaCarouselIndex - 1 + mediaCarouselImages.length) % mediaCarouselImages.length;
      updateMediaCarousel();
   }
   function mediaCarouselNext() {
      mediaCarouselIndex = (mediaCarouselIndex + 1) % mediaCarouselImages.length;
      updateMediaCarousel();
   }
</script>

---

## 📁 Gender Studies

_Designs created for my gender studies courses._

<div id="gender-studies-carousel" style="max-width: 800px; margin: 0 auto; text-align: center;">
   <img id="gender-carousel-image" src="{{ site.baseurl }}/assets/Canva/Gender Studies/1.png" width="300" style="border-radius: 18px; box-shadow: 0 6px 24px rgba(0,0,0,0.18); transition: box-shadow 0.3s, transform 0.3s;" />
   <div style="margin-top: 1rem; display: flex; justify-content: center; gap: 1.5em;">
      <button onclick="genderCarouselPrev()" class="carousel-btn" aria-label="Previous" style="padding: 0.3em 1em; font-size: 0.9em;">
         <span style="font-size: 1.2em; display: inline-block; transform: rotate(-20deg); color: #7b2ff2;">&#8592;</span>
         <span style="font-family: 'Brush Script MT', cursive; font-size: 1em; color: #7b2ff2; margin-left: 0.2em;">Prev</span>
      </button>
      <button onclick="genderCarouselNext()" class="carousel-btn" aria-label="Next" style="padding: 0.3em 1em; font-size: 0.9em;">
         <span style="font-family: 'Brush Script MT', cursive; font-size: 1em; color: #f357a8; margin-right: 0.2em;">Next</span>
         <span style="font-size: 1.2em; display: inline-block; transform: rotate(20deg); color: #f357a8;">&#8594;</span>
      </button>
   </div>
</div>
<script>
   // All images from Canva/Gender Studies
   const genderCarouselImages = [
    {% assign folder = "assets/Canva/Gender Studies" %}
    {% for file in site.static_files %}
      {% if file.path contains folder %}
        {% if file.extname == ".png" or file.extname == ".jpg" or file.extname == ".jpeg" %}
          "{{ site.baseurl }}{{ file.path }}",
        {% endif %}
      {% endif %}
    {% endfor %}
   ];
   let genderCarouselIndex = 0;
   function updateGenderCarousel() {
      document.getElementById('gender-carousel-image').src = genderCarouselImages[genderCarouselIndex];
   }
   function genderCarouselPrev() {
      genderCarouselIndex = (genderCarouselIndex - 1 + genderCarouselImages.length) % genderCarouselImages.length;
      updateGenderCarousel();
   }
   function genderCarouselNext() {
      genderCarouselIndex = (genderCarouselIndex + 1) % genderCarouselImages.length;
      updateGenderCarousel();
   }
</script>






---
