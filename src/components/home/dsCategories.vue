<template>
  <div class="categories">
    <div class="container">
      <div class="categories__inner flex">
        <router-link class="categories__item" to="">
          <div class="categories__item-box">
            <img src="~@/assets/img/categories/category-1.png" alt="Виртуальная реальность">
          </div>
          <div class="categories__item-title">Виртуальная реальность</div>
        </router-link>
        <router-link class="categories__item bottom" to="">
          <div class="categories__item-box">
            <img src="~@/assets/img/categories/category-2.png" alt="Моноподы для селфи">
          </div>
          <div class="categories__item-title">Моноподы <br> для селфи</div>
        </router-link>
        <router-link class="categories__item" to="">
          <div class="categories__item-box">
            <img src="~@/assets/img/categories/category-3.png" alt="Экшн-камеры">
          </div>
          <div class="categories__item-title">Экшн-камеры</div>
        </router-link>
        <router-link class="categories__item" to="">
          <div class="categories__item-box">
            <img src="~@/assets/img/categories/category-4.png" alt="Фитнес-браслеты">
          </div>
          <div class="categories__item-title">Фитнес-браслеты</div>
        </router-link>
        <router-link class="categories__item" to="">
          <div class="categories__item-box">
            <img src="~@/assets/img/categories/category-5.png" alt="Умные часы">
          </div>
          <div class="categories__item-title">Умные часы</div>
        </router-link>
        <router-link class="categories__item" to="">
          <div class="categories__item-box">
            <img src="~@/assets/img/categories/category-6.png" alt="Квадрокоптеры">
          </div>
          <div class="categories__item-title">Квадрокоптеры</div>
        </router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "dsCategories"
}
</script>