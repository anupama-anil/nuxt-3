<template>
  <section>
    <NuxtLayout :name="layout">
      <p>Custom layout in about.vue </p>
    </NuxtLayout>
        <p>This page will be displayed at the /about route.</p>
  </section>  
</template>

<script  setup>
const layout = 'custom'
</script>