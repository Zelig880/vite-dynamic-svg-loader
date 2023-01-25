<script setup>
import iconLoader from './components/iconLoader.vue';
import iconLoaderRaw from './components/iconLoaderRaw.vue';
</script>

<template>
  <div>
    <iconLoader icon="policies" />
    <iconLoaderRaw icon="policies" />
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
