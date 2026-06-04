<script setup lang="ts">
</script>

<template>
  <header class="navigation">
    <div class="navigation-title">
      <h1 class="title-text">VueDex</h1>
    </div>
    <div class="navigation-items">
      <div class="navigation-item">
        <RouterLink class="navigation-item" to="/">
          Home
        </RouterLink>
      </div>
      <div class="navigation-item">
        <RouterLink class="navigation-item" to="route.path">
          Favoritos
        </RouterLink>
      </div>
      <div class="navigation-item">
        <RouterLink class="navigation-item" to="route.path">
          Comparar
        </RouterLink>
      </div>
    </div>
  </header>
</template>

<style scoped>
.navigation {
  display: flex;
  flex-direction: row;
  padding: 0 20px;
  color: var(--title-text-color);
  background-color: var(--primary);
  justify-content: space-between;
  align-items: center;
  height: 56px;
  border-bottom: 2px solid #2060b5;
}

.navigation-title {
  display: flex;
  align-items: center;
}

.title-text {
  margin: 0;
  color: var(--title-text-color);
  font-size: 22px;
  text-decoration: none;
}

.navigation-items {
  display: flex;
  flex-direction: row;
  height: 100%;
}

.navigation-item {
  display: flex;
  align-items: center;
  padding: 0 10px;
  color: var(--title-text-color);
  text-decoration: none;
}

.navigation-item:hover {
  background-color: #ef6666;
  color: var(--secondary);
  text-shadow: 0 0 5px currentColor;
}


</style>