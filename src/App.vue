<script setup>
  import { RouterView } from 'vue-router'
  import ViviBotBrand from './components/icons/ViviBotBrand.vue'
  const links = "text-blue-400 font-bold transition-colors hover:text-blue-100 text-sm font-pp"
  const header = "flex justify-between items-center"
</script>

<template>
  <header :class="header">
    <div>
      <RouterLink to="/">
        <ViviBotBrand />
      </RouterLink>
    </div>
    <div class="flex gap-14">
      <RouterLink :class="links" to="/about">
        About
      </RouterLink>
      <RouterLink :class="links" to="/docs">
        Docs
      </RouterLink>
      <RouterLink :class="links" to="/source">
        Source
      </RouterLink>
    </div>
  </header>
  <RouterView />
</template>

<style scoped>
header {
  background: rgb(0, 0, 0);
  background: linear-gradient(0deg, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 0.7847514005602241) 100%);
  height: 50px;
  padding: 0px 12.361111111111%;
  position: fixed;
  width: 100%;
}

@media  (max-width: 1366px) {
  header  {
    padding: 0px 74px;
  }
}
</style>
