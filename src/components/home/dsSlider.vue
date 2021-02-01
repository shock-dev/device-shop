<template>
  <div class="home__slider">
    <div class="container">
      <hooper>
        <slide>
          <div class="slider__item flex">
            <div class="slider__item-img">
              <img src="~@/assets/img/slider-img.png" alt="">
            </div>
            <div class="slider__item-info">
              <div class="slider__item-head">
                <span>01</span>
              </div>
              <h2 class="slider__item-title">Делай селфи,<br> как Бен Стиллер!</h2>
              <p class="slider__item-text">
                Самая длинная палка для селфи доступна в нашем магазине.
                Восемь (Восемь, Карл!) метров длиной и весом всего 5 килограмм.
              </p>
              <button class="slider__item-button">Подробнее</button>
              <div class="slider__item-params flex">
                <div class="slider__item-params__item">
                  <span>8,5 м</span>
                  <span>Длина палки</span>
                </div>
                <div class="slider__item-params__item">
                  <span>5 кг</span>
                  <span>Вес палки</span>
                </div>
                <div class="slider__item-params__item">
                  <span>Карбон</span>
                  <span>Материал</span>
                </div>
              </div>
            </div>
          </div>
        </slide>
        <slide>
          <div class="slider__item flex">
            <div class="slider__item-img">
              <img src="~@/assets/img/slider-img.png" alt="">
            </div>
            <div class="slider__item-info">
              <div class="slider__item-head">
                <span>01</span>
              </div>
              <h2 class="slider__item-title">Делай селфи,<br> как Бен Стиллер!</h2>
              <p class="slider__item-text">
                Самая длинная палка для селфи доступна в нашем магазине.
                Восемь (Восемь, Карл!) метров длиной и весом всего 5 килограмм.
              </p>
              <button class="slider__item-button">Подробнее</button>
              <div class="slider__item-params flex">
                <div class="slider__item-params__item">
                  <span>8,5 м</span>
                  <span>Длина палки</span>
                </div>
                <div class="slider__item-params__item">
                  <span>5 кг</span>
                  <span>Вес палки</span>
                </div>
                <div class="slider__item-params__item">
                  <span>Карбон</span>
                  <span>Материал</span>
                </div>
              </div>
            </div>
          </div>
        </slide>
        <slide>
          <div class="slider__item flex">
            <div class="slider__item-img">
              <img src="~@/assets/img/slider-img.png" alt="">
            </div>
            <div class="slider__item-info">
              <div class="slider__item-head">
                <span>01</span>
              </div>
              <h2 class="slider__item-title">Делай селфи,<br> как Бен Стиллер!</h2>
              <p class="slider__item-text">
                Самая длинная палка для селфи доступна в нашем магазине.
                Восемь (Восемь, Карл!) метров длиной и весом всего 5 килограмм.
              </p>
              <button class="slider__item-button">Подробнее</button>
              <div class="slider__item-params flex">
                <div class="slider__item-params__item">
                  <span>8,5 м</span>
                  <span>Длина палки</span>
                </div>
                <div class="slider__item-params__item">
                  <span>5 кг</span>
                  <span>Вес палки</span>
                </div>
                <div class="slider__item-params__item">
                  <span>Карбон</span>
                  <span>Материал</span>
                </div>
              </div>
            </div>
          </div>
        </slide>
        <hooper-pagination slot="hooper-addons"></hooper-pagination>
      </hooper>
      </div>
    </div>
</template>

<script>
import {
  Hooper,
  Slide,
  Pagination as HooperPagination
} from 'hooper'
import 'hooper/dist/hooper.css'

export default {
  name: "dsSlider",
  components: {
    Hooper,
    Slide,
    HooperPagination
  }
}
</script>