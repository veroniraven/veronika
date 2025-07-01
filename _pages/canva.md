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

<div id="edmonton-global-carousel" style="max-width: 320px; margin: 0 auto; text-align: center;">
   <img id="carousel-image" src="{{ site.baseurl }}/assets/Canva/Edmonton Global/3.png" width="300" style="border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.1);" />
   <div style="margin-top: 0.5rem;">
      <button onclick="carouselPrev()" style="padding: 0.3em 1em; margin-right: 0.5em;">&#8592; Prev</button>
      <button onclick="carouselNext()" style="padding: 0.3em 1em;">Next &#8594;</button>
   </div>
</div>
<script>
   const carouselImages = [
      "{{ site.baseurl }}/assets/Canva/Edmonton Global/3.png",
      "{{ site.baseurl }}/assets/Canva/Edmonton Global/Amii Media Release.png",
      "{{ site.baseurl }}/assets/Canva/Edmonton Global/Bureau Veritas Cover.png",
      "{{ site.baseurl }}/assets/Canva/Edmonton Global/Global Briefing Sports Image.png",
      "{{ site.baseurl }}/assets/Canva/Edmonton Global/Grengine TAP Illustration.png"
      // Add more image paths here if needed
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
