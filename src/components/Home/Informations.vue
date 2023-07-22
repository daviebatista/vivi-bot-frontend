<script setup>
const section = 'flex flex-col md:flex-row lg:mt-16 justify-between items-center gap-[20%] mt-24'
const img = 'lg:w-96 md:w-72 sm:w-56 w-44'
const div = 'flex flex-col justify-center w-full text-center md:text-left'
const h1 = 'font-pp text-blue-100 text-4xl lg:text-4xl md:text-3xl mt-20'
const p = 'lg:text-2xl md:text-1xl text-2xl text-blue-100 font-ms lg:w-[90%] mt-10'
const strong = 'uppercase text-sm font-light font-ms mt-10 pb-16'
</script>

<template>
  <section :class="section">
    <img src="../icons/vivi-square.svg" alt="vivi-square" :class="img" />
    <div :class="div">
      <h1 :class="h1">
        A <strong>reliable</strong> way to <strong>increment</strong> <br />
        your servers.
      </h1>
      <p :class="p">
        Save time, efforts and money. Vivi Bot is <strong>free</strong> to be used, and will
        <strong>always</strong> be that way.
      </p>
      <strong :class="strong">Current version: 3.3.3</strong>
    </div>
  </section>
</template>

<style scoped>
section {
  background: #000216;
  background: linear-gradient(180deg, #020617 0%, #000 88.02%);
  padding: 0px 12.361111111111%;
  min-height: 100vh;
}

h1 {
  line-height: 52px;
}

strong {
  color: #5c469c;
  font-weight: normal;
}

@media (max-width: 1366px) {
  section {
    padding: 0px 85px;
  }
}

@media (max-width: 1024px) {
  h1 {
    line-height: 36px;
  }
}

@media (max-width: 610px) {
  section {
    padding: 0px 40px;
  }
}

@media (max-width: 420px) {
  h1 {
    font-size: 24px;
  }
}
</style>
