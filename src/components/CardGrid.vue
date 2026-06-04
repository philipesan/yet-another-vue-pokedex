<script setup lang="ts">

</script>

<template>
  <section class="pokemon-grid">
    <slot/>
  </section>
</template>

<style scoped>
.pokemon-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
  gap: 16px;
}
</style>