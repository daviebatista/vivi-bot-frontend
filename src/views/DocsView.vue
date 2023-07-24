<script setup>
import Container from '../components/Container.vue'
import Docs from '../components/Docs/Docs.vue'
</script>

<template>
  <Container>
    <slot>
      <Docs />
    </slot>
  </Container>
</template>

<style></style>
