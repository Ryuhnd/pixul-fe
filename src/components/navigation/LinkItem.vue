<script setup lang="ts">
import { RouterLink } from "vue-router";

type LinkItemType = "logo" | "button" | "standard";

interface LinkItemProps {
  href: string;
  type?: LinkItemType;
}

const { href, type = "button" } = defineProps<LinkItemProps>();
</script>

<template>
  <RouterLink :to="href" class="link" :class="type">
    <slot></slot>
  </RouterLink>
</template>

<style scoped lang="scss">
.link {
  text-decoration: none;
  color: white;
  transition: 0.4s;

  &.router-link-active {
    background: #424242;
  }

  &.logo {
    display: flex;

    :slotted(img) {
      height: var(--logo-height, 32px);
    }
  }

  &.button {
    border: 1px solid grey;
    border-radius: 0.35rem;
    padding: 0.25rem 0.4rem;
  }
}

@media (hover: hover) {
  .link:hover {
    opacity: 0.8;

    &.button {
      opacity: 1;
      background: #313131;
    }
  }
}
</style>
