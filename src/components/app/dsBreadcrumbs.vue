<template>
  <div class="breadcrumbs">
    <ul class="breadcrumbs__list flex">
      <li class="breadcrumbs__item">
        <router-link class="breadcrumbs__link" to="">Главная</router-link>
      </li>
      <li class="breadcrumbs__item">
        <router-link class="breadcrumbs__link" to="">Каталог товаров</router-link>
      </li>
      <li class="breadcrumbs__item">
        <router-link class="breadcrumbs__link" to="">Моноподы для селфи</router-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "dsBreadcrumbs"
}
</script>