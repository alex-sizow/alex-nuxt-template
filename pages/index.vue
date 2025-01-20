<script setup lang="ts">
const route = useRoute();
</script>

<template>
  <main>
    <h1>Alex Sizov</h1>
    <div class="image-container">
      <img src="@/assets/i.webp" alt="" />
    </div>
  </main>
</template>

<style scoped>
main {
  padding: 20px;
}

.image-container {
  width: 600px;
  height: 600px;
  background: green;
  border-radius: 20px;
}
img {
  width: 100%;
  filter: grayscale(100%);
  transition: all 1s ease !important;
  -webkit-filter: grayscale(100%);
  -moz-filter: grayscale(100%);
  transition: filter 0.5s ease-in-out;
  -webkit-transition: -webkit-filter 0.5s ease-in-out;
  -moz-transition: -moz-filter 0.5s ease-in-out;
}

img:hover {
  transition: all 1s ease !important;
  filter: grayscale(0%);
  -webkit-filter: grayscale(0%);
  -moz-filter: grayscale(0%);
}
</style>
