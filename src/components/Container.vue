<template>
  <section class="bg-slate-950 flex flex-col">
    <slot />
  </section>
</template>

<style scoped>
section {
  min-height: 100vh;
}

@media (max-width: 610px) {
  section {
    padding: 130px 0px 0px 0px;
  }
}
</style>
