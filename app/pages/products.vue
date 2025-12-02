<script setup>

</script>

<template>
<div class="products">
 <section class="product-list">
    <nav>
      <ul>
        <li class="navlinks"><NuxtLink to="/about" class="cta-button">About</NuxtLink></li>
        <li class="navlinks"><NuxtLink to="/index" class="cta-button">Home</NuxtLink></li>
        <li class="navlinks"><NuxtLink to="/contact" class="cta-button">Contact</NuxtLink></li>
        <li class="navlinks"><NuxtLink to="/products" class="cta-button">Products</NuxtLink></li>
      </ul>
    </nav>
<h1>Products</h1>
<h2>Camera Equipment</h2>
<img id="product-img" src="/images/camera-equipment.jpg">
<p>
One of the most important things of operating a photography business is selling camera equipment.
At Michael's Photography Studio, we have a full inventory of camera equipment and gear that will be benifical 
to your photography needs! From camera lenses, tri-pods, bags, and many other essential gear, we have everything that 
a photographer can ask for!
</p>
<h2>Photography Lessons</h2>
<img id="product-img" src="/images/photography-lessons.jpg"></img>
<p>
Not only do we sell camera equipment, but we host photography classes too. If you want to take picture in a professional manner,
then these classes are the right thing for you. In these classes, you would learn about the basics of photography such as learning
depth of field, advanced lighting, shutter speeds, textures, and more!
</p>
 </section>   
</div>
</template>

<style>
img {
  max-width: 50%;
  margin: 0;
  padding: 0;
}

h1 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
  text-align: center;
}

.products {
    max-width: 800px;
  margin: 0 auto;
  padding: 2rem;
  font-family: Tahoma, Verdana, sans-serif;
  line-height: 1.6;
}

.navlinks {
  display: inline-block;
  list-style: none;
  gap: 1rem;
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

nav {
    text-align: center;
}
</style>