<script setup lang="ts">

import { useRoute } from 'vue-router';

const route = useRoute()

// When accessing /posts/1, route.params.id will be 1
console.log(route.params.id)
</script>

<template>
    <div class="home-page">
    <section class="intro">
    <h1>Michael Volk's Photography Studio</h1>
    <p>Hi, I'm <strong>Michael Volk.</strong> I'm an Interactive Media Design student at Algonquin College.</p>
  <header>
    <nav>
      <ul>
        <li class="navlinks"><NuxtLink to="/about" class="cta-button">About</NuxtLink></li>
        <li class="navlinks"><NuxtLink to="/photos" class="cta-button">Photos</NuxtLink></li>
        <li class="navlinks"><NuxtLink to="/contact" class="cta-button">Contact</NuxtLink></li>
        <li class="navlinks"><NuxtLink to="/products" class="cta-button">Products</NuxtLink></li>
      </ul>
    </nav>
  </header>
    </section>
    <section class="highlights">
    <h2>Recent Photos</h2>
<ul>
        <li>
          <strong>Paradise</strong>
          <img id="gallery-img" src="/images/IMG_2360.png">
        </li>
        <li>
          <strong>Lighthouse</strong>
          <img id="gallery-img" src="/images/IMG_2626.png">
        </li>
        <li>
          <strong>Village</strong>
          <img id="gallery-img" src="/images/IMG_3828.png">
        </li>
      </ul>
      </section>
    </div>
    <footer>&#169; Michael Volk's Photography Studio 2025</footer>
</template>


<style scoped>
.home-page {
  max-width: 800px;
  margin: 0 auto;
  padding: 2rem;
  font-family: Tahoma, Verdana, sans-serif;
  color: #333;
}

.intro {
  text-align: center;
  margin-bottom: 3rem;
}

.intro h1 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
}

.intro p {
  font-size: 1.2rem;
  margin-bottom: 1.5rem;
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

.highlights h2 {
  font-size: 1.75rem;
  margin-bottom: 1rem;
}

.highlights ul {
  list-style: disc;
  padding-left: 1.5rem;
  margin-bottom: 1rem;
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

img {
  max-width: 100%;
  margin: 0;
  padding: 0;
}

li {
  display: block;
}

.navlinks {
  display: inline-block;
  list-style: none;
  gap: 10px;
}
</style>