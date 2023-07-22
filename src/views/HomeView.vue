<script setup>
import ViviBotBrand from '../components/icons/ViviBotBrand.vue'
import Container from '../components/Container.vue';
</script>

<template>
  <Container>
    <slot>
      <ViviBotBrand/>
    </slot>
  </Container>
</template>

<style scoped>
</style>