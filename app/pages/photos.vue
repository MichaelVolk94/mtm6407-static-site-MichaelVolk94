<script setup>
import { useRoute } from 'vue-router';

const route = useRoute()

// When accessing /posts/1, route.params.id will be 1
console.log(route.params.id)
</script>

<template>
<div class="gallery">
  <header>
   <nav>
      <ul>
        <li class="navlinks"><NuxtLink to="/about" class="cta-button">About</NuxtLink></li>
        <li class="navlinks"><NuxtLink to="/" class="cta-button">Home</NuxtLink></li>
        <li class="navlinks"><NuxtLink to="/contact" class="cta-button">Contact</NuxtLink></li>
        <li class="navlinks"><NuxtLink to="/products" class="cta-button">Products</NuxtLink></li>
      </ul>
    </nav>
<h1>Gallery</h1>
  </header>
</div>
<section class="photo-gallery">
    <h2>Recent Photos</h2>
<ul>
        <li>
          <img id="gallery-img" src="/images/IMG_2360.png">
        </li>
        <li>
          <img id="gallery-img" src="/images/IMG_2626.png">
        </li>
        <li>
          <img id="gallery-img" src="/images/IMG_3828.png">
        </li>
        <li>
          <img id="gallery-img" src="/images/IMG_3912.png">
        </li>
                <li>
          <img id="gallery-img" src="/images/IMG_1842.png">
        </li>
                <li>
          <img id="gallery-img" src="/images/IMG_2240.png">
        </li>
                <li>
          <img id="gallery-img" src="/images/IMG_3484.png">
        </li>
                <li>
          <img id="gallery-img" src="/images/IMG_3639.png">
        </li>
      </ul>
      <footer>&#169; Michael Volk's Photography Studio 2025</footer>
      </section>
</template>

<style scoped>
.gallery {
  max-width: 750px;
  margin: 0 auto;
  padding: 2rem;
  font-family: Tahoma, Verdana, sans-serif;
  text-align: center;
}
.navlinks {
  display: inline-block;
  list-style: none;
  gap: 1rem;
}

.photo-gallery {
  text-align: center;
  margin-bottom: 3rem;
}

img {
  max-width: 90%;
  margin: 0;
  padding: 0;
}

li {
  display: block;
}

h2 {
  font-family: Tahoma, Verdana, sans-serif;
}

.cta-button {
  display: inline-block;
  padding: 0.75rem 1.5rem;
  background-color: #007acc;
  color: white;
  border-radius: 6px;
  text-decoration: none;
  font-weight: bold;
}

.cta-button:hover {
  background-color: #005fa3;
}

.cta-link {
  display: inline-block;
  color: #007acc;
  font-weight: bold;
  text-decoration: none;
  margin-top: 1rem;
}

.cta-link:hover {
  text-decoration: underline;
}
</style>