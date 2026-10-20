<script setup lang="ts">
import NavigationBar from "@/components/navigation/NavigationBar.vue";
</script>

<template>
  <header>
    <NavigationBar />
  </header>
</template>

<style scoped lang="scss">
header {
  height: 65px;
  padding: 0 1rem;
  display: flex;
  align-items: center;
  position: sticky;
  top: 0;
  background-color: #222222;
}

@media (prefers-color-scheme: light) {
  header {
    background-color: white;
  }
}
</style>
