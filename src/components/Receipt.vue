<script setup>
import IconStarsFill from './icons/IconStarsFill.vue'
import IconStarsEmpty from './icons/IconStarsEmpty.vue'
</script>

<template>
  <section class="receipt">
    <div class="container relative">
      <div class="receipt-wrapper d-flex flex-column">
        <h2 class="receipt-title">
          Browser Our Trending <br>
          <span>Receipt</span>
        </h2>
        <div class="receipt-grid d-grid">
          <div class="receipt-card pizza d-flex flex-column align-items-start">
            <img alt="Card Image" class="card-image position-relative" src="./../assets/images/pizza-paperoni.svg" />
            <div class="d-flex flex-column position-relative">
              <p class="card-title">Pizza Paperoni</p>
              <p class="card-category">Pizza</p>
            </div>
            <div class="card-rating position-relative">
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsEmpty />
            </div>
          </div>
          <div class="receipt-card pizza d-flex flex-column align-items-start">
            <img alt="Card Image" class="card-image position-relative" src="./../assets/images/pizza-meat.svg" />
            <div class="d-flex flex-column position-relative">
              <p class="card-title">Pizza Meat</p>
              <p class="card-category">Pizza</p>
            </div>
            <div class="card-rating position-relative">
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsEmpty />
              <IconStarsEmpty />
            </div>
          </div>
          <div class="receipt-card kebab d-flex flex-column align-items-start">
            <img alt="Card Image" class="card-image position-relative" src="./../assets/images/doner-kebab.svg" />
            <div class="d-flex flex-column position-relative">
              <p class="card-title">Doner Kebab</p>
              <p class="card-category">Kebab</p>
            </div>
            <div class="card-rating position-relative">
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsFill />
            </div>
          </div>
          <div class="receipt-card salmon d-flex flex-column align-items-start">
            <img alt="Card Image" class="card-image position-relative" src="./../assets/images/salmon-roll.svg" />
            <div class="d-flex flex-column position-relative">
              <p class="card-title">Salmon Roll</p>
              <p class="card-category">Salmon</p>
            </div>
            <div class="card-rating position-relative">
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsEmpty />
            </div>
          </div>
          <div class="receipt-card cupcake d-flex flex-column align-items-start">
            <img alt="Card Image" class="card-image position-relative" src="./../assets/images/cupcake-choco.svg" />
            <div class="d-flex flex-column position-relative">
              <p class="card-title">Cupcake Choco</p>
              <p class="card-category">Cupcake</p>
            </div>
            <div class="card-rating position-relative">
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsEmpty />
            </div>
          </div>
          <div class="receipt-card doughnut d-flex flex-column align-items-start">
            <img alt="Card Image" class="card-image position-relative" src="./../assets/images/doughnut-milk.svg" />
            <div class="d-flex flex-column position-relative">
              <p class="card-title">Doughnut Milk</p>
              <p class="card-category">Doughnut</p>
            </div>
            <div class="card-rating position-relative">
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsFill />
            </div>
          </div>
          <div class="receipt-card doughnut d-flex flex-column align-items-start">
            <img alt="Card Image" class="card-image position-relative" src="./../assets/images/doughnut-unicorn.svg" />
            <div class="d-flex flex-column position-relative">
              <p class="card-title">Doughnut Unicorn</p>
              <p class="card-category">Doughnut</p>
            </div>
            <div class="card-rating position-relative">
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsEmpty />
            </div>
          </div>
          <div class="receipt-card kebab d-flex flex-column align-items-start">
            <img alt="Card Image" class="card-image position-relative" src="./../assets/images/kathi-kebab.svg" />
            <div class="d-flex flex-column position-relative">
              <p class="card-title">Kathi Kebab</p>
              <p class="card-category">Kebab</p>
            </div>
            <div class="card-rating position-relative">
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsFill />
              <IconStarsEmpty />
            </div>
          </div>
        </div>
        <div class="d-flex justify-content-center">
          <a href="#" class="receipt-button">ALL Receipt</a>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
/* desktop */
.receipt {
  padding: 64px 0 59px;
}

.receipt-wrapper {
  gap: 56px;

}

.receipt-title {
  font-family: Rubik;
  font-size: 38px;
  font-weight: 500;
  line-height: 50px;
  color: var(--vt-c-dark);
}

.receipt-title span {
  color: var(--vt-c-primary);
  font-weight: 500;
}

.receipt-grid {
  grid-template-columns: repeat(4, 1fr);
  gap: 20px 30px;
}

.receipt-card {
  position: relative;
  gap: 19px;
  padding: 33px 20px;
  border-radius: 17px;
  box-shadow: 0px 11px 39px 0px rgba(0, 0, 0, 0.07);
}

.receipt-card.pizza {
  background-color: var(--vt-c-ocean-drift-2);
}

.receipt-card.kebab {
  background-color: var(--vt-c-sky-twilight-2);
}

.receipt-card.cupcake {
  background-color: var(--vt-c-olive-bloom-2);
}

.receipt-card.doughnut {
  background-color: var(--vt-c-moss-glow-2);
}

.receipt-card.salmon {
  background-color: var(--vt-c-berry-crush-2);
}

.receipt-card:before {
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

.receipt-card:hover:before {
  opacity: 5%;
}

.card-title {
  font-family: Rubik;
  font-size: 26px;
  font-weight: 500;
  line-height: 50px;
  color: #000;
}

.card-category {
  font-family: Rubik;
  font-size: 18px;
  font-weight: 500;
  line-height: normal;
  color: var(--vt-c-primary);
}

.receipt-button {
  font-family: Rubik;
  font-size: 14px;
  font-weight: 500;
  line-height: 22px;
  padding: 10px 18px;
  border-radius: 100px;
  align-items: center;
  background-color: var(--vt-c-primary);
  color: var(--vt-c-white);
  box-shadow: 0px 8px 32px 0px rgba(102, 107, 226, 0.35);
}

.receipt-button:hover {
  background-color: var(--vt-c-moss-glow);
}

/* responsive */
@media (max-width: 1199px) {
  .receipt-grid {
    grid-template-columns: repeat(3, 1fr);
  }
}

@media (max-width: 991px) {
  .receipt-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 767px) {
  .receipt-title {
    font-size: 24px;
    line-height: 30px;
  }

  .container {
    padding: 0px 43px 0px 45px;
  }
}

@media (max-width: 575px) {
  .receipt-grid {
    grid-template-columns: repeat(1, 1fr);
  }
}
</style>
