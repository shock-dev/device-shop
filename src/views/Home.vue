<template>
  <div class="home">
    <ds-slider/>
    <ds-categories/>
  </div>
</template>

<script>
import DsSlider from "@/components/home/dsSlider"
import DsCategories from "@/components/home/dsCategories"

export default {
  name: "Home",
  components: {
    DsCategories,
    DsSlider
  }
}
</script>