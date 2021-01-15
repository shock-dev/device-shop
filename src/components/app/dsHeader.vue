<template>
  <header class="header">
    <div class="container">
      <div class="header__inner">
        <router-link class="header__logo" :to="{ name: 'Home' }">
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
                <button class="header__action login">Валентин Петухов</button>
                <button class="header__logout">Выйти</button>
              </div>
              <div class="header__col" v-else>
                <button class="header__action">Войти</button>
              </div>
              <!-- ** -->
              <div class="header__col flex header__additional-buttons">
                <button class="header__action compare">Сравнить</button>
                <button class="header__action cart">Корзина</button>
              </div>
            </div>
          </div>
        </div>
        <div class="header__row align">
          <div class="header__col"></div>
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
