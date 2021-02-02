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
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "dsFooter"
}
</script>