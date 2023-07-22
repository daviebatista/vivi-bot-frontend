<script setup>
import Container from '../components/Container.vue';
import Hero from '../components/Home/Hero.vue';
</script>

<template>
  <Container class="pt-24">
    <slot>
      <Hero/>
    </slot>
  </Container>
</template>

<style scoped>
</style>