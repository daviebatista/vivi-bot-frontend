<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header class="bg-black">
    <div>
      <RouterLink to="/"> Home </RouterLink>
    </div>

    <div>
      <RouterLink to="/about"> About </RouterLink>
      <RouterLink to="/docs"> Docs </RouterLink>
      <RouterLink to="/source"> Source </RouterLink>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
* {
  background-color: black;
}
</style>
