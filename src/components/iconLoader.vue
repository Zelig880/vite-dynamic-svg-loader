<script setup>
    import { ref } from 'vue'
    const props = defineProps({
        icon: String
    })
    const iconName = ref(null);
    
    import(`../assets/${props.icon}.svg`)
      .then((module) => {
        iconName.value = module.default;
      })
      .catch(console.error.bind(console));
</script>

<template>
    <component :is="iconName" />
</template>
