<script setup>
import { RouterView } from 'vue-router'
import ViviBotBrand from './components/icons/ViviBotBrand.vue'
const links = 'text-blue-400 font-bold transition-colors hover:text-blue-200 text-sm font-pp'
const header = 'flex flex-row justify-between items-center fixed h-[50px] w-full'
const hoverLogo = 'hover:brightness-125 transition-all'
</script>

<template>
  <header :class="header">
    <div>
      <RouterLink to="/" :class="hoverLogo">
        <ViviBotBrand />
      </RouterLink>
    </div>
    <div class="flex gap-14">
      <RouterLink :class="links" to="/about"> About </RouterLink>
      <RouterLink :class="links" to="/docs"> Docs </RouterLink>
      <RouterLink :class="links" to="/source"> Source </RouterLink>
    </div>
  </header>
  <RouterView />
</template>

<style scoped>
header {
  background: rgb(0, 0, 0);
  background: linear-gradient(0deg, rgba(0, 0, 0, 0.09007352941176472) 0%, rgba(0, 0, 0, 1) 89%);
  padding: 0px 12.361111111111%;
}

@media (max-width: 1366px) {
  header {
    padding: 0px 74px;
  }
}

@media (max-width: 610px) {
  header {
    background: linear-gradient(0deg, rgba(0, 0, 0, 0.6138830532212884) 0%, rgba(0, 0, 0, 1) 100%);
    flex-direction: column;
    gap: 10px;
    height: 100px;
    padding: 10px 74px;
  }
}
</style>
