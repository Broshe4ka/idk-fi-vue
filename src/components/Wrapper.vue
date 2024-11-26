<script setup lang="ts">
import Header from './Layout/Header.vue';
import Toolbar from './Layout/Toolbar.vue';
</script>

<template>
  <div class="wrapper">
    <Header />
    <Toolbar />
    <img
      src="https://i.pinimg.com/originals/86/8b/e7/868be70af8ebf3c9a8552c3409aa3919.png"
      alt=""
      class="wrapper__img"
    />
  </div>
</template>

<style lang="scss">
.wrapper {
  position: relative;

  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;

  width: 100%;
  height: 100%;
  border-radius: 1rem;

  &__img {
    position: absolute;
    width: 100%;
    height: 100%;
    object-fit: cover;
    z-index: -1;
    border-radius: inherit;
  }
}
</style>
