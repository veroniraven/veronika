---
layout: single
title: "Canva Portfolio"
permalink: /canva/
author_profile: true
---

Welcome to my Canva design portfolio! Below are collections of my visual work, organized by project or topic.

---

## 📁 Edmonton Global

_A collection of designs themed around the Edmonton Global project._

<div id="edmonton-global-carousel" style="max-width: 800px; margin: 0 auto; text-align: center;">
   <img id="carousel-image" src="{{ site.baseurl }}/assets/Canva/Edmonton Global/3.png" width="600" style="border-radius: 18px; box-shadow: 0 6px 24px rgba(0,0,0,0.18); transition: box-shadow 0.3s, transform 0.3s;" />
   <div style="margin-top: 1rem; display: flex; justify-content: center; gap: 1.5em;">
      <button onclick="carouselPrev()" class="carousel-btn" aria-label="Previous">
         <span style="font-size: 2em; display: inline-block; transform: rotate(-20deg); color: #7b2ff2;">&#8592;</span>
         <span style="font-family: 'Brush Script MT', cursive; font-size: 1.2em; color: #7b2ff2; margin-left: 0.3em;">Prev</span>
      </button>
      <button onclick="carouselNext()" class="carousel-btn" aria-label="Next">
         <span style="font-family: 'Brush Script MT', cursive; font-size: 1.2em; color: #f357a8; margin-right: 0.3em;">Next</span>
         <span style="font-size: 2em; display: inline-block; transform: rotate(20deg); color: #f357a8;">&#8594;</span>
      </button>
   </div>
</div>
<style>
  .carousel-btn {
    background: linear-gradient(90deg, #fbc2eb 0%, #a6c1ee 100%);
    border: none;
    border-radius: 2em;
    padding: 0.6em 2em;
    box-shadow: 0 2px 12px rgba(123,47,242,0.08);
    cursor: pointer;
    transition: transform 0.15s, box-shadow 0.15s;
    margin: 0 0.5em;
    display: flex;
    align-items: center;
    gap: 0.2em;
  }
  .carousel-btn:hover {
    transform: scale(1.07) rotate(-2deg);
    box-shadow: 0 4px 24px rgba(243,87,168,0.16);
  }
</style>
<script>
   // All images from Canva/Edmonton Global
   const carouselImages = [
      "{{ site.baseurl }}/assets/Canva/Edmonton Global/3.png",
      "{{ site.baseurl }}/assets/Canva/Edmonton Global/Amii Media Release.png",
      "{{ site.baseurl }}/assets/Canva/Edmonton Global/Bureau Veritas Cover.png",
      "{{ site.baseurl }}/assets/Canva/Edmonton Global/Global Briefing Sports Image.png",
      "{{ site.baseurl }}/assets/Canva/Edmonton Global/Grengine TAP Illustration.png",
      "{{ site.baseurl }}/assets/Canva/Edmonton Global/Happy Canada Day Instagram Post.png",
      "{{ site.baseurl }}/assets/Canva/Edmonton Global/IXON Social Post.png",
      "{{ site.baseurl }}/assets/Canva/Edmonton Global/National Indigenous Peoples Day.png",
      "{{ site.baseurl }}/assets/Canva/Edmonton Global/Open Farm Days 1.png",
      "{{ site.baseurl }}/assets/Canva/Edmonton Global/Open Farm Days 2.png",
      "{{ site.baseurl }}/assets/Canva/Edmonton Global/RWI Trade Heroes.png",
      "{{ site.baseurl }}/assets/Canva/Edmonton Global/Title Page.png",
      "{{ site.baseurl }}/assets/Canva/Edmonton Global/Webinar Recap Cover.png"
   ];
   let carouselIndex = 0;
   function updateCarousel() {
      document.getElementById('carousel-image').src = carouselImages[carouselIndex];
   }
   function carouselPrev() {
      carouselIndex = (carouselIndex - 1 + carouselImages.length) % carouselImages.length;
      updateCarousel();
   }
   function carouselNext() {
      carouselIndex = (carouselIndex + 1) % carouselImages.length;
      updateCarousel();
   }
</script>
---

## 📁 Gender Studies

_Digital materials and visual assets focused on gender studies._

👉 *(Add designs or embedded visuals here)*

---

## 📁 Media Studies

_Designs related to media literacy, analysis, and presentation._

👉 *(Add previews or links from this folder here)*

---

## 📄 DUSS Year-in-Review

[Download the PDF report](/assets/images/canva/duss_year-in-review.pdf)

---
