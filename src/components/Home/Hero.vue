<script setup>
import Buttons from '../Buttons/Buttons.vue'
const section = 'flex flex-col items-center gap-10'
const div = 'flex flex-col items-center gap-12'
const text1 =
  'font-semibold font-ms text-3xl text-blue-50 text-center flex flex-col gap-3 leading-11 sm:text-4xl lg:text-5xl'
const text2 =
  'font-bold font-ms text-2xl text-blue-50 text-center flex flex-col gap-3 leading-7 sm:text-3xl lg:text-4xl'
</script>

<template>
  <section :class="section">
    <div :class="div">
      <div :class="text1">
        <h1>Your personal</h1>
        <h1>Discord Bot Experience</h1>
      </div>
      <img
        src="../icons/vivi-icon.svg"
        alt="icon"
        class="w-20 border-blue-400 border-4 rounded-full"
      />
      <div :class="text2">
        <h1>Introducing Vivi Bot, your</h1>
        <h1>customizable gaming companion</h1>
      </div>
    </div>
    <Buttons />
  </section>
</template>

<style scoped></style>
