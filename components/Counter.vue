<script setup>
const count = ref(0);
const Increase = () => {
  count.value++;
};
const Decrease = () => {
  count.value--;
};
</script>
<template>
  <button @click="Increase">Increase</button>
  <p>{{ count }}</p>
  <button @click="Decrease">Decrease</button>
</template>
