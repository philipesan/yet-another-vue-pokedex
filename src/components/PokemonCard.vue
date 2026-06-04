<script setup lang="ts">
import pokeball from '@/assets/pokeball.svg'
import pokeballLine from '@/assets/pokeball-nonfavorite.svg'
</script>

<template>
  <article class="pokemon-card">
    <button class="favorite-button">
      <img class="pokemon-favorite" :src="pokeballLine" alt="Favorite" />
    </button>
    <img class="pokemon-image" alt="Spritework" />

    <h2 class="pokemon-name">
      Pikachu
    </h2>
    <div class="pokemon-types">
      <span class="type-badge"> Electric </span>
    </div>
    <RouterLink class="details-button" to="details">
      <span class="details-text">See More!</span>
    </RouterLink>
  </article>
</template>

<style scoped>
  .pokemon-card {
    position: relative;
    background: #fff;
    border: 1px solid #e4e7eb;
    border-radius: 18px;
    padding: 16px;
    text-align: center;
  }

  .pokemon-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 8px 24px rgba(0, 0, 0, 0.08);
  }

  .favorite-button {
    position: absolute;
    top: 12px;
    right: 12px;
    border: none;
    background: transparent;
    font-size: 20px;
    cursor: pointer;
  }

  .pokemon-favorite {
    width: 20px;
    height: 20px;
    display: inline-block;
  }

  .pokemon-image {
    width: 120px;
    height: 120px;
    object-fit: contain;
  }

  .pokemon-name {
    margin: 8px 0;
    font-size: 18px;
    text-transform: capitalize;
  }

  .pokemon-types {
    margin: 10px 0 20px 0;
    display: flex;
    justify-content: center;
    gap: 8px;
    flex-wrap: wrap;
  }

  .type-badge {
    padding: 4px 8px;
    border-radius: 999px;
    background: #f3f4f6;
    font-size: 12px;
  }
  .details-button {
    margin: 10px;
    padding: 4px 8px;
    border-radius: 999px;
    background: var(--primary);
  }

  .details-text {
    display: inline-block;
    font-size: 12px;
    text-decoration: none;
    color: #ffffff;
    font-weight: bold;
  }
</style>