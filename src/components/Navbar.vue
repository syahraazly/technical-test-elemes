<script setup>

</script>

<template>
  <header class="navbar">
    <div class="container">
      <div class="navbar-wrapper">
        <a href="#">
          <img alt="Elmes logo" class="logo" src="./../assets/images/brand-logo.svg" />
        </a>
        <div class="navbar-links">
          <a href="#" class="links-item">Home</a>
          <a href="#" class="links-item">About</a>
          <a href="#" class="links-item highlighted">
            Promotions
            <span>HOT</span>
          </a>
          <a href="#" class="links-item">Blogs</a>
          <a href="#" class="links-item">Contact Us</a>
        </div>
        <div class="navbar-buttons">
          <a href="#" class="login">Masuk</a>
          <a href="#" class="register">Daftar Sekarang</a>
        </div>
      </div>
    </div>
  </header>
</template>

<style scoped>
/* desktop */
.navbar {
  padding: 19px 0 27px;
  background: transparent;
  position: absolute;
  width: 100%;
  z-index: 10;
}

.navbar-wrapper {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 48px;
  width: 100%;
}

.navbar-links {
  display: flex;
  align-items: center;
  gap: 32px;
}

.links-item {
  position: relative;
  font-family: Rubik;
  font-size: 14px;
  font-weight: 500;
  line-height: 22px;
  color: var(--vt-c-dark-40);
}

.links-item:hover {
  color: var(--vt-c-dark);
}

.links-item.highlighted span {
  position: absolute;
  right: -15px;
  top: -18px;
  padding: 3px 9px 2px;
  background: #E7462D;
  border-radius: 8px;
  font-family: Open Sans;
  font-size: 8px;
  font-weight: 700;
  line-height: 14px;
  color: var(--vt-c-white);
}

.navbar-buttons {
  display: flex;
  align-items: center;
  gap: 24px;
}

.navbar-buttons a {
  font-family: Rubik;
  font-size: 14px;
  font-weight: 500;
  line-height: 22px;
}

.navbar-buttons .login {
  color: var(--vt-c-dark);
}

.navbar-buttons .login:hover {
  color: var(--vt-c-dark-40);
}

.navbar-buttons .register {
  padding: 10px 18px;
  border-radius: 100px;
  align-items: center;
  background-color: var(--vt-c-primary);
  color: var(--vt-c-white);
}

.navbar-buttons .register:hover {
  background-color: var(--vt-c-moss-glow);
}

/* responsive */
@media (max-width: 991px) {
  .navbar-links {
    display: none;
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
