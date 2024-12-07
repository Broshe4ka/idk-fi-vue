<script setup lang="ts">
import SettingsWrapper from '../SettingsWrapper.vue';
</script>

<template>
  <div class="menu__wrapper">
    <SettingsWrapper />
    <div class="menu">
      <div class="player">
        <div class="player__controls">
          <button class="control__button">
            <img
              src="/icons/prev.svg"
              alt="Prev"
              class="button__img"
            />
          </button>
          <button class="control__button">
            <img
              src="/icons/pause.svg"
              alt="Pause"
              class="button__img"
            />
          </button>
          <button class="control__button">
            <img
              src="/icons/next.svg"
              alt="Next"
              class="button__img"
            />
          </button>
        </div>
        <div class="player__song">
          <div class="song__title">
            Kurt Cobain - And i love her
          </div>
        </div>
      </div>
      <div class="menu__controls">
        <button class="control__button">
          <img src="/icons/sound.svg" alt="" />
        </button>
        <button class="control__button">
          <img src="/icons/wrapper.svg" alt="" />
        </button>
        <button class="control__button">
          <img src="/icons/settings.svg" alt="" />
        </button>
        <button class="control__button">
          <img src="/icons/burger.svg" alt="" />
        </button>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.menu {
  position: relative;

  padding: 1rem 1.5rem;
  display: flex;
  align-items: center;
  gap: 2rem;

  border-radius: 1rem 1rem 0 0;
  background: var(--main-bg);

  &__wrapper {
    display: flex;
    flex-direction: column;
    gap: 1rem;
    z-index: var(--z-index-higher);
  }

  &__controls {
    display: flex;
    gap: 0.5rem;
  }
  &::after,
  &::before {
    content: '';
    position: absolute;
    bottom: 0;

    width: 1rem;
    height: 1rem;

    background: url(/icons/rec.svg);
  }

  &::after {
    left: -1rem;
    transform: rotate(-90deg);
  }
  &::before {
    right: -1rem;
  }
}
.player {
  display: flex;
  align-items: center;
  gap: 1.25rem;
  &__controls {
    display: flex;
    gap: 0.25rem;
  }
  &__song {
    width: 15.25rem;
    font-size: 14px;
    font-style: normal;
    line-height: 1rem;
    font-weight: 300;

    padding: 0.5rem 0.75rem;

    background: var(--hovered-bg);
    border-radius: 0.75rem;
  }
}

.control__button {
  width: 2rem;
  padding: 0.25rem;
  aspect-ratio: 1/1;

  display: flex;
  align-items: center;
  justify-content: center;

  border-radius: 0.75rem;
  transition: var(--ease-transition);
  &:hover {
    background: var(--hovered-bg);
  }
}
</style>
