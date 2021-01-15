<template>
  <header class="header">
    <div class="container">
      <div class="header__inner">
        <router-link class="header__logo" :to="{ name: 'Home' }">
          <img src="~@/assets/img/logo.png" alt="Logo">
        </router-link>
        <div class="header__row">
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
                <button class="header__username">Валентин Петухов</button>
                <button class="header__logout">Выйти</button>
              </div>
              <div class="header__col" v-else>
                <button class="header__login">Войти</button>
              </div>
            </div>
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
