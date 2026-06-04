<script setup lang="ts">
import AppHeader from "@/components/AppHeader.vue";
import PokemonCard from "@/components/PokemonCard.vue";
import PokemonSearch from "@/components/PokemonSearch.vue";
import PokemonTypeFilter from "@/components/PokemonTypeFilter.vue";
import CardGrid from "@/components/CardGrid.vue";
import LoadMoreButton from "@/components/LoadMoreButton.vue";
</script>
<template>
  <AppHeader />
  <div class="container">
    <PokemonSearch />
    <PokemonTypeFilter />
    <CardGrid>
      <PokemonCard/>
      <PokemonCard/>
      <PokemonCard/>
      <PokemonCard/>
      <PokemonCard/>
      <PokemonCard/>
      <PokemonCard/>
      <PokemonCard/>
      <PokemonCard/>
      <PokemonCard/>
      <PokemonCard/>
      <PokemonCard/>
    </CardGrid>
    <LoadMoreButton />
  </div>


</template>

<style scoped>

</style>