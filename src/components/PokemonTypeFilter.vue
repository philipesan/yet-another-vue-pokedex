<script setup lang="ts">

</script>

<template>
  <p class="pokemon-search-title">Popular Types:</p>
  <div class="pokemon-types">
    <button class="type-button"> Dragon </button>
    <button class="type-button"> Fairy </button>
    <button class="type-button"> Dark </button>
    <button class="type-button"> Fire </button>
  </div>
</template>

<style scoped>
.pokemon-types {
  margin: 10px 0 20px 0;
  display: flex;
  justify-content: center;
  gap: 8px;
  flex-wrap: wrap;
}

.pokemon-search-title {
  font-weight: 600;
  color: var(--strong-text)
}

.type-button {
  flex: 1;
  padding: 10px 12px;
  border-radius: 18px;
  border: 0 solid var(--primary);
  color: #fff;
  background-color: var(--primary);
}

.type-button:hover {
  background-color: #ef6666;
  text-shadow: 0 0 5px currentColor;
}
</style>