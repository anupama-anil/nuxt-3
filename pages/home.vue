<template>
  <div>
    <NuxtLayout name="mainlayout">
      <template #header> Some header template content in the component. </template>
      The rest of the page
    </NuxtLayout>
  </div>
</template>

<script setup>
definePageMeta({
  layout: false,
});
</script>
