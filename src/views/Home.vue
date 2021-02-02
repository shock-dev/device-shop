<template>
  <div class="home">
    <ds-slider/>
    <ds-categories/>
    <ds-services/>
    <ds-brands/>
    <ds-feedback/>
  </div>
</template>

<script>
import DsSlider from "@/components/home/dsSlider"
import DsCategories from "@/components/home/dsCategories"
import DsServices from "@/components/home/dsServices"
import DsBrands from "@/components/home/dsBrands"
import DsFeedback from "@/components/home/dsFeedback";

export default {
  name: "Home",
  components: {
    DsFeedback,
    DsBrands,
    DsServices,
    DsCategories,
    DsSlider
  }
}
</script>