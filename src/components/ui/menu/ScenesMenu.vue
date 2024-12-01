<script setup lang="ts"></script>

<!-- #TODO: Make scene as component -->

<template>
  <div class="scenes">
    <div class="scene">
      <span class="scene__title">Lakehouse</span>
      <div class="scene__icons">
        <img
          src="/icons/scenes-icons/sunset.svg"
          alt="Scene icon"
          class="icon"
        />
        <img
          src="/icons/scenes-icons/birds.svg"
          alt="Scene icon"
          class="icon"
        />
        <img
          src="/icons/scenes-icons/waves.svg"
          alt="Scene icon"
          class="icon"
        />
      </div>
      <img
        src="https://lofi-co-assets.vexcited.com/wallpapers/Fuji/fuji2.jpg"
        alt=""
        class="scene__bg"
      />
    </div>
    <div class="scene">
      <span class="scene__title">Lakehouse</span>
      <div class="scene__icons">
        <img
          src="/icons/scenes-icons/sunset.svg"
          alt="Scene icon"
          class="icon"
        />
        <img
          src="/icons/scenes-icons/birds.svg"
          alt="Scene icon"
          class="icon"
        />
        <img
          src="/icons/scenes-icons/waves.svg"
          alt="Scene icon"
          class="icon"
        />
      </div>
      <img
        src="https://lofi-co-assets.vexcited.com/wallpapers/Fuji/fuji2.jpg"
        alt=""
        class="scene__bg"
      />
    </div>
    <div class="scene">
      <span class="scene__title">Lakehouse</span>
      <div class="scene__icons">
        <img
          src="/icons/scenes-icons/sunset.svg"
          alt="Scene icon"
          class="icon"
        />
        <img
          src="/icons/scenes-icons/birds.svg"
          alt="Scene icon"
          class="icon"
        />
        <img
          src="/icons/scenes-icons/waves.svg"
          alt="Scene icon"
          class="icon"
        />
      </div>
      <img
        src="https://lofi-co-assets.vexcited.com/wallpapers/Fuji/fuji2.jpg"
        alt=""
        class="scene__bg"
      />
    </div>
    <div class="scene">
      <span class="scene__title">Lakehouse</span>
      <div class="scene__icons">
        <img
          src="/icons/scenes-icons/sunset.svg"
          alt="Scene icon"
          class="icon"
        />
        <img
          src="/icons/scenes-icons/birds.svg"
          alt="Scene icon"
          class="icon"
        />
        <img
          src="/icons/scenes-icons/waves.svg"
          alt="Scene icon"
          class="icon"
        />
      </div>
      <img
        src="https://lofi-co-assets.vexcited.com/wallpapers/Fuji/fuji2.jpg"
        alt=""
        class="scene__bg"
      />
    </div>
  </div>
</template>

<style scoped lang="scss">
.scenes {
  display: flex;
  gap: 0.75rem;

  overflow-x: scroll;
}
.icon {
  display: block;
  width: 2rem;
  height: 2rem;
}
.scene {
  position: relative;

  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 1.25rem;

  border-radius: 0.5rem;

  padding: 2rem 1.25rem 0.75rem 1.25rem;

  background: linear-gradient(
    0deg,
    rgba(0, 0, 0, 0.55) 0%,
    rgba(0, 0, 0, 0.55) 100%
  );
  &__title {
    font-size: 2rem;
    font-weight: 500;
    line-height: 1rem;
    letter-spacing: -1.92px;
  }
  &__icons {
    display: flex;
    gap: 0.75rem;
    align-items: center;
    justify-content: center;
  }
  &__bg {
    position: absolute;
    top: 0;
    left: 0;

    width: 100%;
    height: 100%;

    border-radius: inherit;

    object-fit: cover;
    z-index: -1;
  }
}
</style>
