<template>
  <div class="home__slider">
    <div class="container">
      <hooper>
        <slide>
          slide 1
        </slide>
        <slide>
          slide 2
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