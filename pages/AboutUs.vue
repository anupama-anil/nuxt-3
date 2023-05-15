<template>
  <section>
    <NuxtLayout :name="layout">
      <p>Custom layout in about.vue</p>
    </NuxtLayout>
    <p>This page will be displayed at the /about route.</p>

    <nav>
      <ul>
        <li><NuxtLink to="/AboutUs">About</NuxtLink></li>
        <li><NuxtLink to="/posts/1">Post 1</NuxtLink></li>
        <li><NuxtLink to="/posts/2">Post 2</NuxtLink></li>
      </ul>
    </nav>
  </section>
</template>

<script setup>
const layout = "custom";
</script>
