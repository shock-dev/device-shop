<template>
  <footer class="footer">
    <div class="container">
      <div class="footer__inner">
        <div class="footer__head">
          <router-link class="footer__logo" to="">
            <img src="~@/assets/img/footer-logo.png" alt="Logo">
          </router-link>
          <div class="footer__actions flex">
            <button class="footer__action">
              <svg class="footer__action-svg" width="13" height="12">
                <use href="~@/assets/img/svg/sprite.svg#login"></use>
              </svg>
              <span class="footer__action-text">Войти</span>
            </button>
            <button class="footer__action">
              <svg class="footer__action-svg" width="10" height="10">
                <use href="~@/assets/img/svg/sprite.svg#compare"></use>
              </svg>
              <span class="footer__action-text">Сравнить</span>
            </button>
            <button class="footer__action">
              <svg class="footer__action-svg" width="12" height="12">
                <use href="~@/assets/img/svg/sprite.svg#cart"></use>
              </svg>
              <span class="footer__action-text">Корзина</span>
            </button>
          </div>
        </div>
        <div class="footer__body">
          <div class="footer__address">г. Москва, ул. Строителей, 15</div>
          <ul class="footer__menu">
            <li class="footer__menu-item">
              <router-link class="footer__menu-link" to="">Доставка</router-link>
            </li>
            <li class="footer__menu-item">
              <router-link class="footer__menu-link" to="">Гарантия</router-link>
            </li>
            <li class="footer__menu-item">
              <router-link class="footer__menu-link" to="">Контакты</router-link>
            </li>
          </ul>
          <div class="footer__phone">Тел.: +7 (495) 495-95-95</div>
        </div>
        <div class="footer__bottom">
          <div class="footer__line"></div>
          <ul class="footer__social flex">
            <li class="footer__social-item">
              <router-link class="footer__social-link" to="">
                <img src="~@/assets/img/svg/fb.svg" alt="Facebook">
              </router-link>
            </li>
            <li class="footer__social-item">
              <router-link class="footer__social-link" to="">
                <img src="~@/assets/img/svg/vk.svg" alt="Vk">
              </router-link>
            </li>
            <li class="footer__social-item">
              <router-link class="footer__social-link" to="">
                <img src="~@/assets/img/svg/twitter.svg" alt="Twitter">
              </router-link>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "dsFooter"
}
</script>