<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header class="header">
    <RouterLink class="nam-link" to="/">Home</RouterLink>
    <RouterLink class="nam-link" to="/about">About</RouterLink>
  </header>

  <div class="route">
    <RouterView />
  </div>
</template>

<style scoped>
.nam-link {
  display: inline-block;
  padding: 11px;
}

.header .router-link-active {
  /* color: red; */
  background-color: #d0ffd6;
}

.route {
  padding-top: 33px;
}
</style>
