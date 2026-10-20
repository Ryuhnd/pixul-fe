<script setup lang="ts">
import LinkItem from "./LinkItem.vue";
</script>
<template>
  <div class="left">
    <LinkItem href="/" type="logo">
      <img alt="Vue logo" src="@/assets/pixul-logo.svg" />
    </LinkItem>

    <LinkItem href="/counter">
      <p>Counter</p>
    </LinkItem>

    <LinkItem href="/games">
      <p>Game List</p>
    </LinkItem>

    <LinkItem href="/admin/games">
      <p>Manage Games</p>
    </LinkItem>
  </div>
</template>
<style scoped lang="scss">
.left {
  display: flex;
  align-items: center;
  gap: 0.5rem;
}
</style>
