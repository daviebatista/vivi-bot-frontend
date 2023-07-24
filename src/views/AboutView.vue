<script setup>
import Container from '../components/Container.vue'
import Hero from '../components/About/Hero.vue'
import About from '../components/About/About.vue'
</script>

<template>
  <Container>
    <slot>
      <Hero />
      <About />
    </slot>
  </Container>
</template>

<style scoped></style>
