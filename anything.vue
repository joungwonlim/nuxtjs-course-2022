<template>
  <div>
    <div>
      <a href="#" @click="changePage('home')" class="">home</a> |
      <a href="#" @click="changePage('counter')" class="">counter</a> |
    </div>
    <Nuxtpage />
    <HomeWelcome v-if="page === 'home'" />
    <LazyCounter v-if="page === 'counter'" />
  </div>
</template>
<script setup>
const page = ref("home");
const changePage = (name) => {
  console.log(name);
  page.value = name;
};
</script>
