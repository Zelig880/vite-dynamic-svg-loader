<script setup>
    import { ref } from 'vue'
    const props = defineProps({
        icon: String
    })
    const iconContent = ref(null);

    import(`../assets/${props.icon}.svg?raw`)
      .then((module) => {
        iconContent.value = module.default;
      })
      .catch(console.error.bind(console));
</script>

<template>
    <span v-html="iconContent">

    </span>
</template>
