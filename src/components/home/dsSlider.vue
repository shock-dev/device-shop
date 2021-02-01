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
                <span>02</span>
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