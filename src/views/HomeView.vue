<script setup>
import Container from '../components/Container.vue'
import Hero from '../components/Home/Hero.vue'
import Informations from '../components/Home/Informations.vue'
import Features from '../components/Home/Features.vue'
import Contribute from '../components/Home/Contribute.vue'
</script>

<template>
  <Container class="pt-24">
    <slot>
      <Hero />
      <Informations />
      <Features />
      <Contribute />
    </slot>
  </Container>
</template>

<style scoped></style>
