<template>
  <div class="home">
    <ds-slider/>
    <ds-categories/>
    <ds-services/>
  </div>
</template>

<script>
import DsSlider from "@/components/home/dsSlider"
import DsCategories from "@/components/home/dsCategories"
import DsServices from "@/components/home/dsServices"

export default {
  name: "Home",
  components: {
    DsServices,
    DsCategories,
    DsSlider
  }
}
</script>