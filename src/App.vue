<script setup>
import headpage from './components/headpage.vue'
import innerpage from './components/innerpage.vue'
</script>

<template>
  <header class="full-page" id="page-header">
    <headpage></headpage>
  </header>

  <main class="layout">
    <innerpage></innerpage>
    <innerpage></innerpage>
    <innerpage></innerpage>
    <innerpage></innerpage>
    <innerpage></innerpage>
    <innerpage></innerpage>
  </main>
</template>

<style scoped>
header.full-page {
  height: 100vh;
  background-attachment: fixed;
  background-image: url('../public/index.jpg');
  color: white;
}

#page-header {
  position: relative;
  width: 100%;
  background-position: center center;
  background-size: cover;
  background-repeat: no-repeat;

}

.layout {
  flex: 1 auto;
  margin: 0 auto;
  padding: 40px 15px;
  max-width: 1200px;
  width: 100%;
}
</style>
