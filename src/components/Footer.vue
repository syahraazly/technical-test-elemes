<script setup>
import IconMail from './icons/IconMail.vue'
import IconCall from './icons/IconCall.vue'
import IconInstagram from './icons/IconInstagram.vue'
</script>

<template>
  <footer class="footer">
    <div class="container">
      <div class="footer-wrapper">
        <div class="footer-card">
          <div class="footer-col-info">
            <div class="info-head">
              <img alt="Elmes logo" class="logo" src="./../assets/images/brand-logo.svg" />
              <p class="info-address">
                Jl. Prof. DR. Satrio No.7, RT.3/RW.3, Karet Kuningan, <br>
                Kecamatan Setiabudi, Kota Jakarta Selatan, <br>
                Daerah Khusus Ibukota Jakarta 12950
              </p>
            </div>
            <div class="info-socials">
              <a href="#" class="social-item">
                <IconMail />
              </a>
              <a href="#" class="social-item">
                <IconCall />
              </a>
              <a href="#" class="social-item">
                <IconInstagram />
              </a>
            </div>
          </div>
          <div class="footer-group">
            <p class="footer-group-title">Categories</p>
            <div class="footer-links">
              <a href="#" class="footer-link">Cupcake</a>
              <a href="#" class="footer-link">Pizza</a>
              <a href="#" class="footer-link">Kebab</a>
              <a href="#" class="footer-link">Salmon</a>
              <a href="#" class="footer-link">Dougnut</a>
            </div>
          </div>
          <div class="footer-group">
            <p class="footer-group-title">About Us</p>
            <div class="footer-links">
              <a href="#" class="footer-link">About Us</a>
              <a href="#" class="footer-link">FAQ</a>
              <a href="#" class="footer-link">Report Problem</a>
            </div>
          </div>
          <div class="footer-group">
            <p class="footer-group-title">Newsletter</p>
            <div class="footer-newsletter">
              <p class="newsletter-text">Get now free 50% discount for alll products on your first order</p>
              <form action="#" class="newsletter-form">
                <input type="text" placeholder="Your email address">
                <button type="submit">SEND</button>
              </form>
              <div class="footer-contact d-flex flex-column">
                <div class="footer-contact-item d-flex align-items-center">
                  <IconMail />
                  <p>elemesid@gmail.com</p>
                </div>
                <div class="footer-contact-item d-flex align-items-center">
                  <IconCall />
                  <p>0888 1111 2222</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <p class="footer-copyright">© 2021 Elemes id. All rights reserved</p>
      </div>
    </div>
  </footer>
</template>

<style scoped>
/* desktop */
.footer {
  margin-top: 191px;
}

.footer-wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 48px;
}

.footer-card {
  padding: 79px 67px 40px 62px;
  background-color: #F9FFF6;
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  gap: 64px;
  border-radius: 20px;
  width: 100%;
}

.footer-copyright {
  font-family: Rubik;
  font-size: 12px;
  font-weight: 400;
  line-height: 16px;
  letter-spacing: 0.6px;
  text-transform: uppercase;
  color: var(--vt-c-dark-40);
}

.footer-col-info {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 33px;
}

.info-head {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 16px;
}

.logo {
  object-fit: cover;
  width: 207px;
  height: 50px;
}

.info-address {
  font-family: Rubik;
  font-size: 14px;
  font-weight: 400;
  line-height: 20px;
  color: var(--vt-c-dark-40);
  max-width: 335px;
}

.info-socials {
  display: flex;
  align-items: center;
  gap: 8px;
}

.info-socials .social-item {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 10px;
  border-radius: 24px;
  background-color: transparent;
  transition: all .4s linear;
}

.info-socials .social-item svg {
  color: var(--vt-c-primary);
  transition: all .2s linear;
}

.info-socials .social-item:hover {
  background-color: var(--vt-c-primary);
}

.info-socials .social-item:hover svg {
  color: var(--vt-c-white);
}

.footer-group {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 33px;
}

.footer-group-title {
  font-family: Rubik;
  font-size: 18px;
  font-weight: 500;
  line-height: 24px;
  color: var(--vt-c-dark);
}

.footer-links {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 19px;
}

.footer-link {
  font-family: Rubik;
  font-size: 14px;
  font-weight: 400;
  line-height: 16px;
  color: var(--vt-c-dark-40);
}

.footer-link:hover {
  color: var(--vt-c-dark);
}

.footer-newsletter {
  display: flex;
  flex-direction: column;
  align-items: stretch;
  gap: 19px;
}

.newsletter-text {
  font-family: Rubik;
  font-size: 14px;
  font-weight: 400;
  line-height: 16px;
  color: var(--vt-c-dark-40);
  max-width: 245px;
}

.newsletter-form {
  display: flex;
  align-items: center;
}

.newsletter-form input {
  border-top-left-radius: 8px;
  border-bottom-left-radius: 8px;
  border: 1px solid #000;
  border-right: none;
  padding: 8px 0px 4px 15px;
  font-family: Rubik;
  font-size: 14px;
  font-weight: 400;
  line-height: 24px;
  color: #000;
  height: 40px;
}

.newsletter-form button {
  height: 40px;
  border-top-right-radius: 8px;
  border-bottom-right-radius: 8px;
  padding: 8px 8px 9px 11px;
  font-family: Rubik;
  font-size: 14px;
  font-weight: 500;
  line-height: 24px;
  color: var(--vt-c-white);
  background-color: var(--vt-c-primary);
  transition: all .2s linear;
}

.newsletter-form button:hover {
  background-color: var(--vt-c-moss-glow);
}

.footer-contact {
  gap: 10px;
}

.footer-contact-item svg {
  color: var(--vt-c-primary);
}

.footer-contact-item p {
  font-family: Rubik;
  font-size: 14px;
  font-weight: 400;
  line-height: 24px;
  color: #000;
}


/* responsive */
@media (max-width: 1199px) {
  .footer-card {
    gap: 24px;
  }
}

@media (max-width: 991px) {
  .footer-card {
    flex-wrap: wrap;
  }

  .footer-col-info {
    width: 100%;
  }
}

@media (max-width: 767px) {
  .footer {
    display: none;
  }
}
</style>
