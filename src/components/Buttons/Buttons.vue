<script setup>
import ContributeButton from './ContributeButton.vue'
import FeaturesButton from './FeaturesButton.vue'
import GetButton from './GetButton.vue'

const div = 'flex flex-row gap-10 flex-wrap justify-center'
const linkHover = 'hover:brightness-150 transition-all'
</script>

<template>
  <div :class="div">
    <a href="" :class="linkHover">
      <FeaturesButton />
    </a>
    <a href="" :class="linkHover">
      <GetButton />
    </a>
    <a href="" :class="linkHover">
      <ContributeButton />
    </a>
  </div>
</template>
