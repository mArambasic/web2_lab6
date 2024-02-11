<script setup>
import { onMounted } from 'vue'
import HomeView from './views/HomeView.vue';

onMounted(() => {
  console.log
  (`Resetting regitration data`)
})
</script>

<template>
  <header>
    <div class="wrapper">
      <HomeView/>

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/hotels">Hotels</RouterLink>
      </nav>
    </div>
  </header>
</template>

<style scoped>

</style>
