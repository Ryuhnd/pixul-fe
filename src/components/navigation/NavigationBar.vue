<script setup lang="ts">
import NavLeftGroup from "./NavLeftGroup.vue";
import NavRightGroup from "./NavRightGroup.vue";
</script>

<template>
  <nav>
    <NavLeftGroup />
    <NavRightGroup />
  </nav>
</template>

<style scoped lang="scss">
nav {
  flex: 1;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
</style>
