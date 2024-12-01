<script setup lang="ts"></script>

<template>
  <div class="settings">
    <div class="volume">
      <div class="volume__title">Master volume</div>
      <div class="volume__items">
        <div class="volume__item">
          <div class="item__header">
            <img
              src="/public/icons/scenes-icons/keyboard.svg"
              alt=""
              class="header__icon"
            />
            <span class="header__title"> Keyboard typing </span>
          </div>
          <div class="item__range">
            <img
              src="/public/icons/sound.svg"
              alt=""
              class="range__icon"
            />
            <input
              type="range"
              min="0"
              max="100"
              step="1"
              class="range__input"
            />
            <span class="range__info"> 100% </span>
          </div>
        </div>
        <div class="volume__item">
          <div class="item__header">
            <img
              src="/public/icons/scenes-icons/keyboard.svg"
              alt=""
              class="header__icon"
            />
            <span class="header__title"> Keyboard typing </span>
          </div>
          <div class="item__range">
            <img
              src="/public/icons/sound.svg"
              alt=""
              class="range__icon"
            />
            <input
              type="range"
              min="0"
              max="100"
              step="1"
              class="range__input"
            />
            <span class="range__info"> 100% </span>
          </div>
        </div>
        <div class="volume__item">
          <div class="item__header">
            <img
              src="/public/icons/scenes-icons/keyboard.svg"
              alt=""
              class="header__icon"
            />
            <span class="header__title"> Keyboard typing </span>
          </div>
          <div class="item__range">
            <img
              src="/public/icons/sound.svg"
              alt=""
              class="range__icon"
            />
            <input
              type="range"
              min="0"
              max="100"
              step="1"
              class="range__input"
            />
            <span class="range__info"> 100% </span>
          </div>
        </div>
      </div>
    </div>
    <div class="scene">
      <div class="scene__radio">
        <span class="radio__title"> Time </span>
        <div class="radio">
          <div class="radio__item">
            <input
              type="radio"
              name="time"
              id="day"
              class="radio__radio"
            />
            <label for="day" class="radio__label noselect">
              <img
                src="/public/icons/sun.svg"
                alt=""
                class="lable__img"
              />
            </label>
          </div>
          <span class="radio__border"></span>
          <div class="radio__item">
            <input
              type="radio"
              name="time"
              id="time_auto"
              class="radio__radio"
            />
            <label
              for="time_auto"
              class="radio__label noselect"
            >
              Auto
            </label>
          </div>
          <span class="radio__border"></span>
          <div class="radio__item">
            <input
              type="radio"
              name="time"
              id="night"
              class="radio__radio"
            />
            <label for="night" class="radio__label noselect">
              <img
                src="/public/icons/moon.svg"
                alt=""
                class="lable__img"
              />
            </label>
          </div>
        </div>
      </div>
    </div>

    <div class="scene__radio">
      <span class="radio__title"> Cycle </span>
      <div class="radio">
        <div class="radio__item">
          <input
            type="radio"
            name="cicle"
            id="sun"
            class="radio__radio"
          />
          <label for="sun" class="radio__label noselect">
            <img
              src="/public/icons/sunny.svg"
              alt=""
              class="lable__img"
            />
          </label>
        </div>
        <span class="radio__border"></span>
        <div class="radio__item">
          <input
            type="radio"
            name="cicle"
            id="cycle_auto"
            class="radio__radio"
          />
          <label for="cycle_auto" class="radio__label noselect">
            Auto
          </label>
        </div>
        <span class="radio__border"></span>
        <div class="radio__item">
          <input
            type="radio"
            name="cicle"
            id="wather"
            class="radio__radio"
          />
          <label for="wather" class="radio__label noselect">
            <img
              src="/public/icons/rain.svg"
              alt=""
              class="lable__img"
            />
          </label>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.settings {
  width: 100%;
  display: flex;
  justify-content: space-between;
}
.volume {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 1rem;

  &__title {
    font-size: 1.5rem;
    font-weight: 500;
    letter-spacing: -1.44px;
  }
  &__items {
    display: flex;
    flex-direction: column;
    gap: 0.75rem;
  }
  &__item {
    display: flex;
    flex-direction: column;
    gap: 0.25rem;
  }
}

.item {
  &__header {
    display: flex;
    align-items: center;
    gap: 0.25rem;
  }
  &__range {
    display: flex;
    align-items: center;
    gap: 0.7rem;
    padding: 0.25rem 0.75rem;
    background: #11111180;
    border-radius: 6px;
  }
}
.header {
  &__icon {
    width: 1.25rem;
    height: 1.25rem;
  }
  &__title {
    letter-spacing: -0.8px;
  }
}
.range {
  &__icon {
    width: 1rem;
    height: 1rem;
  }
  &__input {
    // #TODO: Style input
  }
  &__info {
    font-size: 0.75rem;
    font-weight: 500;
    line-height: 1rem;
    letter-spacing: -0.72px;
  }
}

.scene {
  display: flex;
  align-items: flex-start;
  gap: 1rem;
  &__radio {
    display: flex;
    flex-direction: column;
    gap: 0.25rem;
  }
}
.radio {
  display: flex;
  align-items: center;
  padding: 5px 6px;
  gap: 0.25rem;
  border-radius: 0.75rem;
  background: rgba(17, 17, 17, 0.5);
  &__title {
    font-size: 1.5rem;
    font-weight: 500;
    letter-spacing: -1.44px;
  }
  &__item {
    display: flex;
  }
  &__border {
    display: block;
    width: 2px;
    height: 1rem;
    background: #525252;
    border-radius: 0.75rem;
  }
  &__radio {
    -webkit-appearance: none;
    appearance: none;
    &:checked + .radio__label {
      background: rgba(255, 255, 255, 0.25);
    }
  }
  &__label {
    cursor: pointer;
    line-height: 24px;
    padding: 2px;
    border-radius: 0.5rem;
    transition: var(--ease-transition);
  }
}
.lable {
  &__img {
  }
}
</style>
