<template>
  <h1>Hello it's post {{ route.params.id }} component</h1>
</template>

<script setup>
const route = useRoute();
// When accessing /posts/1, route.params.id will be 1
console.log(route.params.id);

definePageMeta({
  middleware: [
    function (to, from) {
      if (to.params.id === "1") {
        return abortNavigation();
      }
      if (to.path !== "3") {
        return navigateTo("/");
      }
    },
  ],

  validate: async (route) => {
    // Check if the id is made up of digits
    return /^\d+$/.test(route.params.id)
  }
});
</script>
