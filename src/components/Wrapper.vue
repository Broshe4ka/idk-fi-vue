<script setup lang="ts">
import Header from './Layout/Header.vue';
import Scene from './Scene.vue';
import Menu from './Layout/Menu.vue';
</script>

<template>
  <div class="wrapper">
    <Header />
    <Menu />
    <Scene />
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
}
</style>
