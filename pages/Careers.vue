<template>
  <section>
    <NuxtLayout :name="layout">
      <p>Custom layout in Carers.vue </p>
    </NuxtLayout>
        <p>This page will be displayed at the /carrers route.</p>
  </section>  
</template>

<script  setup>
definePageMeta({
  layout: "custom",
});
</script>