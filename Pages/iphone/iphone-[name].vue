<template>
  <div>iphone {{ name }}</div>
</template>
<script setup>
const route = useRoute();
const name = computed(() => {
  return route.params.name.replaceAll("-", " ");
});
</script>
