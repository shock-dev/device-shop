<template>
  <header class="header">
    <div class="container">
      <div class="header__inner">
        <router-link class="header__logo" :to="{ name: 'Catalog' }">
          <img src="~@/assets/img/logo.png" alt="Logo">
        </router-link>
        <div class="header__row align">
          <div class="header__col search flex" :class="{ active: searchActive }">
            <label class="search__label">
              <input
                class="search__input"
                type="text"
                placeholder="Поиск по сайту"
                @focus="searchActive = true"
                @focusout="searchActive = false"
              >
            </label>
            <button class="search__btn">Найти</button>
          </div>
          <div class="header__col">
            <div class="header__row">
              <div class="header__col" v-if="auth">
                <button class="header__action">
                  <svg class="header__action-svg" width="13" height="12">
                    <use href="~@/assets/img/svg/sprite.svg#login"></use>
                  </svg>
                  <span class="header__action-text">Валентин Петухов</span>
                </button>
                <button class="header__logout">Выйти</button>
              </div>
              <div class="header__col" v-else>
                <button class="header__action">
                  <svg class="header__action-svg" width="13" height="12">
                    <use href="~@/assets/img/svg/sprite.svg#login"></use>
                  </svg>
                  <span class="header__action-text">Войти</span>
                </button>
              </div>
              <!-- ** -->
              <div class="header__col flex header__additional-buttons">
                <button class="header__action">
                  <svg class="header__action-svg" width="10" height="10">
                    <use href="~@/assets/img/svg/sprite.svg#compare"></use>
                  </svg>
                  <span class="header__action-text">Сравнить</span>
                </button>
                <button class="header__action">
                  <svg class="header__action-svg" width="12" height="12">
                    <use href="~@/assets/img/svg/sprite.svg#cart"></use>
                  </svg>
                  <span class="header__action-text">Корзина</span>
                </button>
              </div>
            </div>
          </div>
        </div>
        <div class="header__row align">
          <div class="header__col">
            <div class="header__catalog">
              <router-link class="header__catalog-title" to="/catalog">Каталог</router-link>
              <div class="header__catalog-popup catalog-popup">
                <div class="catalog-popup__inner flex">
                  <ul class="catalog-popup__list">
                    <li class="catalog-popup__item">
                      <router-link class="catalog-popup__link" to="#">Виртуальная реальность</router-link>
                    </li>
                    <li class="catalog-popup__item">
                      <router-link class="catalog-popup__link" to="#">Моноподы для селфи</router-link>
                    </li>
                    <li class="catalog-popup__item">
                      <router-link class="catalog-popup__link" to="#">Экшн-камеры</router-link>
                    </li>
                  </ul>
                  <ul class="catalog-popup__list">
                    <li class="catalog-popup__item">
                      <router-link class="catalog-popup__link" to="#">Фитнеc-браслеты</router-link>
                    </li>
                    <li class="catalog-popup__item">
                      <router-link class="catalog-popup__link" to="#">Умные часы</router-link>
                    </li>
                  </ul>
                  <ul class="catalog-popup__list">
                    <li class="catalog-popup__item">
                      <router-link class="catalog-popup__link" to="#">Квадрокоптеры</router-link>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </div>
          <div class="header__col">
            <nav class="header__menu menu">
              <ul class="menu__list flex">
                <li class="menu__item">
                  <router-link class="menu__link" to="#">Доставка</router-link>
                </li>
                <li class="menu__item">
                  <router-link class="menu__link" to="#">Гарантия</router-link>
                </li>
                <li class="menu__item">
                  <router-link class="menu__link" to="#">Контакты</router-link>
                </li>
              </ul>
            </nav>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "dsHeader",
  data: () => ({
    searchActive: false,
    auth: true
  })
}
</script>
