<template>
   <div class="header">
    Hellooo it's custom layout
    <slot />
  </div>
</template>

<style scoped>
/* Header/Logo Title */
.header {
  padding: 60px;
  text-align: center;
  background: #da2357;
  color: white;
  font-size: 30px;
}
</style>