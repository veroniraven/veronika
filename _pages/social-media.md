---
layout: single
title: "Social Media Posts"
permalink: /social-media/
author_profile: true
---

<div id="social-media-carousel" style="max-width: 800px; margin: 0 auto; text-align: center;">
    <img id="social-carousel-image" src="{{ site.baseurl }}/assets/Social Media Posts Edmonton Global/Amii Media Release Post.png" width="600" style="border-radius: 18px; box-shadow: 0 6px 24px rgba(0,0,0,0.18); transition: box-shadow 0.3s, transform 0.3s;" />
    <div style="margin-top: 1rem; display: flex; justify-content: center; gap: 1.5em;">
        <button onclick="socialCarouselPrev()" class="carousel-btn" aria-label="Previous" style="padding: 0.3em 1em; font-size: 0.9em;">
            <span style="font-size: 1.2em; display: inline-block; transform: rotate(-20deg); color: #7b2ff2;">&#8592;</span>
            <span style="font-family: 'Brush Script MT', cursive; font-size: 1em; color: #7b2ff2; margin-left: 0.2em;">Prev</span>
        </button>
        <button onclick="socialCarouselNext()" class="carousel-btn" aria-label="Next" style="padding: 0.3em 1em; font-size: 0.9em;">
            <span style="font-family: 'Brush Script MT', cursive; font-size: 1em; color: #f357a8; margin-right: 0.2em;">Next</span>
            <span style="font-size: 1.2em; display: inline-block; transform: rotate(20deg); color: #f357a8;">&#8594;</span>
        </button>
    </div>
</div>
<script>
const socialCarouselImages = [
     {% assign folder = "assets/Social Media Posts Edmonton Global" %}
     {% for file in site.static_files %}
        {% if file.path contains folder %}
          {% if file.extname == ".png" or file.extname == ".jpg" or file.extname == ".jpeg" %}
             "{{ site.baseurl }}{{ file.path }}",
          {% endif %}
        {% endif %}
     {% endfor %}
];
let socialCarouselIndex = 0;
function updateSocialCarousel() {
    document.getElementById('social-carousel-image').src = socialCarouselImages[socialCarouselIndex];
}
function socialCarouselPrev() {
    socialCarouselIndex = (socialCarouselIndex - 1 + socialCarouselImages.length) % socialCarouselImages.length;
    updateSocialCarousel();
}
function socialCarouselNext() {
    socialCarouselIndex = (socialCarouselIndex + 1) % socialCarouselImages.length;
    updateSocialCarousel();
}
</script>
