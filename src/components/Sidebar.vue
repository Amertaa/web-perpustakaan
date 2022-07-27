<template>
  <aside>
    <div class="logo">
      <ion-icon name="logo-github" size="large"></ion-icon>
    </div>

    <div class="menu-toggle-wrap">
      <button class="menu-toggle">
        <ion-icon name="chevron-forward-outline" size="small" @click="ToggleMenu"></ion-icon>
      </button>
    </div>
  </aside>
</template>

<script setup>
import { ref } from 'vue';

const Togglemenu = () => {};
</script>

<style lang="scss" scoped>
aside {
  display: flex;
  flex-direction: column;
  width: calc(2rem + 32px);
  overflow: hidden;
  min-height: 100vh;
  padding: 1rem;

  background-color: var(--dark);
  color: var(--light-color);

  transition: 0.2s ease-out;

  @media (max-width: 768px) {
    position: fixed;
    z-index: 99;
  }
}
</style>
