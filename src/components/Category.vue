<script setup>
import IconStarsFill from './icons/IconStarsFill.vue'
import IconStarsEmpty from './icons/IconStarsEmpty.vue'
import { VueperSlides, VueperSlide } from 'vueperslides'
import 'vueperslides/dist/vueperslides.css'
import './customVueper.css'

import { ref, computed, onMounted, onUnmounted } from "vue";
const slider = ref(null);
// Reactive screen width
const screenWidth = ref(window.innerWidth);

// Method to update screen width
const updateScreenWidth = () => {
  screenWidth.value = window.innerWidth;
};

// Add or remove the event listener
onMounted(() => {
  window.addEventListener("resize", updateScreenWidth);
});

onUnmounted(() => {
  window.removeEventListener("resize", updateScreenWidth);
});

// Computed properties for arrows and bullets visibility
const showArrows = computed(() => screenWidth.value >= 768);
const showBullets = computed(() => screenWidth.value < 768);
const visibleSlides = computed(() => {
  if (screenWidth.value < 575) {
    return 1.5;
  } else if (screenWidth.value < 768) {
    return 1.5;
  } else if (screenWidth.value < 992) {
    return 2.8;
  } else if (screenWidth.value < 1200) {
    return 3.8;
  } else {
    return 5;
  }
});
</script>

<template>
  <section class="category">
    <div class="container relative">
      <div class="category-wrapper d-flex flex-column">
        <h2 class="category-title">
          Browser Our Category <br>
          <span>Receipt</span>
        </h2>
        <div class="category-slider d-flex flex-column">
          <vueper-slides class="no-shadow" :visible-slides="visibleSlides" :arrows="showArrows" :gap="1"
            :bullets="false" :class="custom - slider" :touchable="showBullets" :dragging-distance="70" prevent-y-scroll>
            <vueper-slide>
              <template #content>
                <div class="carousel-card cupcake">
                  <img alt="Card Image" class="carousel-card-image" src="./../assets/icons/icon-muffin.svg" />
                  <div class="carousel-card-contet d-flex flex-column align-items-center">
                    <p class="carousel-card-title">Cupcake</p>
                    <p class="carousel-card-desc">22 Items</p>
                  </div>
                </div>
              </template>
            </vueper-slide>
            <vueper-slide>
              <template #content>
                <div class="carousel-card pizza">
                  <img alt="Card Image" class="carousel-card-image" src="./../assets/icons/icon-pizza.svg" />
                  <div class="carousel-card-contet d-flex flex-column align-items-center">
                    <p class="carousel-card-title">Pizza</p>
                    <p class="carousel-card-desc">25 Items</p>
                  </div>
                </div>
              </template>
            </vueper-slide>
            <vueper-slide>
              <template #content>
                <div class="carousel-card kebab">
                  <img alt="Card Image" class="carousel-card-image" src="./../assets/icons/icon-kebab.svg" />
                  <div class="carousel-card-contet d-flex flex-column align-items-center">
                    <p class="carousel-card-title">Kebab</p>
                    <p class="carousel-card-desc">12 Items</p>
                  </div>
                </div>
              </template>
            </vueper-slide>
            <vueper-slide>
              <template #content>
                <div class="carousel-card salmon">
                  <img alt="Card Image" class="carousel-card-image" src="./../assets/icons/icon-salmon.svg" />
                  <div class="carousel-card-contet d-flex flex-column align-items-center">
                    <p class="carousel-card-title">Salmon</p>
                    <p class="carousel-card-desc">22 Items</p>
                  </div>
                </div>
              </template>
            </vueper-slide>
            <vueper-slide>
              <template #content>
                <div class="carousel-card doughnut">
                  <img alt="Card Image" class="carousel-card-image" src="./../assets/icons/icon-doughnut.svg" />
                  <div class="carousel-card-contet d-flex flex-column align-items-center">
                    <p class="carousel-card-title">Doughnut</p>
                    <p class="carousel-card-desc">11 Items</p>
                  </div>
                </div>
              </template>
            </vueper-slide>
            <vueper-slide>
              <template #content>
                <div class="carousel-card cupcake">
                  <img alt="Card Image" class="carousel-card-image" src="./../assets/icons/icon-muffin.svg" />
                  <div class="carousel-card-contet d-flex flex-column align-items-center">
                    <p class="carousel-card-title">Cupcake</p>
                    <p class="carousel-card-desc">22 Items</p>
                  </div>
                </div>
              </template>
            </vueper-slide>
            <vueper-slide>
              <template #content>
                <div class="carousel-card pizza">
                  <img alt="Card Image" class="carousel-card-image" src="./../assets/icons/icon-pizza.svg" />
                  <div class="carousel-card-contet d-flex flex-column align-items-center">
                    <p class="carousel-card-title">Pizza</p>
                    <p class="carousel-card-desc">25 Items</p>
                  </div>
                </div>
              </template>
            </vueper-slide>
            <vueper-slide>
              <template #content>
                <div class="carousel-card kebab">
                  <img alt="Card Image" class="carousel-card-image" src="./../assets/icons/icon-kebab.svg" />
                  <div class="carousel-card-contet d-flex flex-column align-items-center">
                    <p class="carousel-card-title">Kebab</p>
                    <p class="carousel-card-desc">12 Items</p>
                  </div>
                </div>
              </template>
            </vueper-slide>
            <vueper-slide>
              <template #content>
                <div class="carousel-card salmon">
                  <img alt="Card Image" class="carousel-card-image" src="./../assets/icons/icon-salmon.svg" />
                  <div class="carousel-card-contet d-flex flex-column align-items-center">
                    <p class="carousel-card-title">Salmon</p>
                    <p class="carousel-card-desc">22 Items</p>
                  </div>
                </div>
              </template>
            </vueper-slide>
            <vueper-slide>
              <template #content>
                <div class="carousel-card doughnut">
                  <img alt="Card Image" class="carousel-card-image" src="./../assets/icons/icon-doughnut.svg" />
                  <div class="carousel-card-contet d-flex flex-column align-items-center">
                    <p class="carousel-card-title">Doughnut</p>
                    <p class="carousel-card-desc">11 Items</p>
                  </div>
                </div>
              </template>
            </vueper-slide>
            <template #arrow-left>
              <button class="category-slider-button" @click="goToPrevSlide">
                <img alt="Card Image" class="" src="./../assets/icons/icon-arrow-left.svg" />
                PREV
              </button>
            </template>

            <template #arrow-right>
              <button class="category-slider-button" @click="goToNextSlide">
                NEXT
                <img alt="Card Image" class="" src="./../assets/icons/icon-arrow-right.svg" />
              </button>
            </template>
          </vueper-slides>
        </div>
        <div class="d-flex justify-content-center">
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
/* desktop */
.category {
  padding: 64px 0 59px;
  overflow: hidden;
}

.category-wrapper {
  gap: 56px;

}

.category-title {
  font-family: Rubik;
  font-size: 38px;
  font-weight: 500;
  line-height: 50px;
  color: var(--vt-c-dark);
}

.category-title span {
  color: var(--vt-c-primary);
  font-weight: 500;
}

.category-slider {
  gap: 10px;
}

.category-slider-buttons {
  gap: 13px;
}

.category-slider-button {
  font-family: Rubik;
  font-size: 14px;
  font-weight: 500;
  line-height: 22px;
  padding: 9px 13px;
  border-radius: 100px;
  align-items: center;
  background-color: var(--vt-c-primary);
  color: var(--vt-c-white);
  box-shadow: 0px 8px 32px 0px rgba(102, 107, 226, 0.35);
}

.category-slider-button:hover {
  background-color: var(--vt-c-moss-glow);
}

.carousel-card {
  position: relative;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 31px;
  padding: 30px 64px;
  border-radius: 8px;
  width: 230px;
  height: 100%;
  max-height: 175px;
  transition: max-height .2s linear;
}

.carousel-card.pizza {
  background-color: var(--vt-c-ocean-drift-2);
}

.carousel-card.kebab {
  background-color: var(--vt-c-sky-twilight-2);
}

.carousel-card.cupcake {
  background-color: var(--vt-c-olive-bloom-2);
}

.carousel-card.doughnut {
  background-color: var(--vt-c-moss-glow-2);
}

.carousel-card.salmon {
  background-color: var(--vt-c-berry-crush-2);
}

.carousel-card:before {
  content: '';
  display: block;
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  opacity: 0%;
  background-color: transparent;
  background-image: url('../assets/images/card-bg.svg');
  background-repeat: no-repeat;
  background-position: 50% 0;
  background-size: auto;
  z-index: 0;
  transition: all .2s linear;
}

.carousel-card:hover {
  max-height: 195px;
}

.carousel-card:hover:before {
  opacity: 5%;
}

.carousel-card-contet {
  gap: 4px;
}

.carousel-card-image {
  height: 47px;
}

.carousel-card-title {
  font-family: Rubik;
  font-size: 16px;
  font-weight: 500;
  line-height: 22px;
  color: var(--vt-c-dark);
}

.carousel-card-desc {
  font-family: Rubik;
  font-size: 14px;
  font-weight: 400;
  line-height: 16px;
  color: var(--vt-c-dark);
}

/* responsive */
@media (max-width: 1199px) {
  .category-grid {
    grid-template-columns: repeat(3, 1fr);
  }
}

@media (max-width: 991px) {
  .category-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 767px) {
  .category-title {
    font-size: 24px;
    line-height: 30px;
  }

  .container {
    padding: 0px 43px 0px 45px;
  }
}

@media (max-width: 575px) {
  .category-grid {
    grid-template-columns: repeat(1, 1fr);
  }
}
</style>
