<script setup lang="ts">

</script>

<template>
  <div class="load-more-footer">
    <button class="load-more-button ">Load More!</button>
  </div>
</template>

<style scoped>
.load-more-footer {
  display: flex;
  flex-direction: row;
  padding: 0 20px;
  color: var(--title-text-color);
  justify-content: center;
  align-items: center;
  height: 56px;
}

.load-more-button {
  padding: 10px 16px;
  width: 80%;
  cursor: pointer;
  border-radius: 18px;
  border-width : 0;
  background-color: var(--primary);
  color: #ffffff;
}

.load-more-button:hover {
  background-color: #ef6666;
  text-shadow: 0 0 5px currentColor;
}
</style>