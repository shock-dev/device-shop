<template>
  <div class="home">
    <ds-slider/>
    <ds-categories/>
    <ds-services/>
    <ds-brands/>
  </div>
</template>

<script>
import DsSlider from "@/components/home/dsSlider"
import DsCategories from "@/components/home/dsCategories"
import DsServices from "@/components/home/dsServices"
import DsBrands from "@/components/home/dsBrands"

export default {
  name: "Home",
  components: {
    DsBrands,
    DsServices,
    DsCategories,
    DsSlider
  }
}
</script>