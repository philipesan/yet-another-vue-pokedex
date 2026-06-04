<script setup lang="ts">
import { ref } from 'vue';

const searchTerm = ref('');

function handleSearch() {
  const value = searchTerm.value.trim();

  if(!value){
    return
  }

  console.log(value)
}
</script>

<template>
  <form class="pokemon-search" @submit.prevent="handleSearch">
  <label for="pokemon-search-input" class="pokemon-search-label">
    Find a Pokemon!
  </label>
    <div class="pokemon-search-controls">
      <input
          id="pokemon-search-input"
          v-model="searchTerm"
          class="pokemon-search-input"
          type="text"
          placeholder="Type a Pokemon Species or Pokédex Number"
      />

      <button class="pokemon-search-button" type="submit">
        Find It!
      </button>
    </div>
  </form>
</template>

<style scoped>
.pokemon-search {
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.pokemon-search-label {
  font-weight: 600;
}

.pokemon-search-controls {
  display: flex;
  gap: 8px;
}

.pokemon-search-input {
  flex: 1;
  padding: 10px 12px;
  border-radius: 18px;
  border: 1px solid var(--primary);
}

.pokemon-search-input:focus {
  outline: none;
  border-color: var(--secondary);
}

.pokemon-search-button {
  padding: 10px 16px;
  cursor: pointer;
  border-radius: 18px;
  border-width : 0;
  background-color: var(--primary);
  color: #ffffff;
}

.pokemon-search-button:hover {
  background-color: #ef6666;
  text-shadow: 0 0 5px currentColor;
}
</style>