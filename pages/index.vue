<template>
  <div>
    <NuxtLayout> <p>Default layout in index.vue</p></NuxtLayout>
    <h1>Welcome to home page</h1>
    <AppAlert><h3>This is an alert component auto imported</h3></AppAlert>

    <div>
      <button @click="enableCustomLayout">Update to custom layout</button>
      <button @click="enableDefaultLayout">Update to default layout</button>
    </div>
  </div>
</template>

<script setup>
definePageMeta({
  pageTransition: {
    name: 'rotate'
  }
})
function enableCustomLayout() {
  setPageLayout("custom");
}
function enableDefaultLayout() {
  setPageLayout('default')
}
useHead({
  title: 'My App',
   link: [
    {
      rel: 'preconnect',
      href: 'https://fonts.googleapis.com'
    },
    {
      rel: 'stylesheet',
      href: 'https://fonts.googleapis.com/css2?family=Roboto&display=swap',
      crossorigin: ''
    }
  ],
  meta: [
    { name: 'description', content: 'My amazing site.' }
  ],
  bodyAttrs: {
    class: 'test'
  },
  script: [ { innerHTML: 'console.log(\'Hello world\')' } ]
})
</script>
