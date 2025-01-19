<script setup>

</script>

<template>
  <section class="hero">
    <div class="container relative">
      <div class="hero-wrapper d-flex align-items-center">
        <div class="hero-contet d-flex flex-column align-items-start">
          <h1 class="hero-title">Good Food Us Good Mood</h1>
          <img alt="Hero Illustration" class="mobile-illustration d-none"
            src="./../assets/images/hero-illustration-mobile.png" />
          <p class="hero-desc">I would think that conserving our natural resources should be a conservative position:
            Not to waste food, and not to throw away a lot of the food that we buy.</p>
          <div class="hero-buttons d-flex align-items-center">
            <button class="register">Daftar Sekarang</button>
            <button class="about">About Us</button>
          </div>
        </div>
        <img alt="Hero Illustration" class="hero-illustration" src="./../assets/images/hero-illustration.png" />
      </div>
    </div>
    <div class="hero-background"></div>
  </section>
</template>

<style scoped>
/* desktop */
.hero {
  padding: 37px 0px 0px;
  /* background: url('../assets/images/hero-bg.svg') rgba(0,0,0, 0.5) no-repeat center;
    background-size: cover; */
  position: relative;
  width: 100%;
}

.hero:before {
  content: '';
  display: block;
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  opacity: 2%;
  background-image: url('../assets/images/hero-bg.svg');
  background-repeat: no-repeat;
  background-position: 50% 0;
  background-size: cover;
  z-index: -1;
}

.hero-wrapper {
  gap: 99px;
}

.hero-contet {
  gap: 32px;
}

.hero-title {
  font-family: Rubik;
  font-size: 64px;
  font-weight: 500;
  line-height: 64px;
  color: var(--vt-c-primary);
}

.hero-desc {
  font-family: Rubik;
  font-size: 18px;
  font-weight: 400;
  line-height: 29px;
  color: var(--vt-c-dark-40);
}

.hero-buttons {
  gap: 16px;
}

.hero-buttons .register {
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

.hero-buttons .register:hover {
  background-color: var(--vt-c-moss-glow);
}

.hero-buttons .about {
  font-family: Rubik;
  font-size: 14px;
  font-weight: 500;
  line-height: 22px;
  padding: 10px 18px;
  border-radius: 100px;
  align-items: center;
  background-color: var(--vt-c-lightgray);
  color: var(--vt-c-dark);
}

/* responsive */
@media (max-width: 991px) {
  .hero {
    padding: 134px 0px 0px;
  }

  .hero .container {
    padding: 0px 34px 0px 28px;
  }

  .hero-illustration {
    display: none;
  }

  .mobile-illustration {
    display: block !important;
    width: 100%;
  }

  .hero-title {
    font-family: Rubik;
    font-size: 48px;
    font-weight: 500;
    line-height: 64px;
    color: var(--vt-c-primary);
  }
}

@media (max-width: 767px) {
  .logo {
    width: 150px;
    height: 36px;
  }
}

@media (max-width: 575px) {
  .navbar-buttons .login {
    display: none;
  }

  .navbar {
    padding: 28px 0 19px;
  }

  .container {
    padding: 0 33px;
  }

  .navbar-wrapper {
    gap: 12px;
  }
}
</style>
