<template>
  <div class="container">
    <div class="row feedback">
      <div class="col-50 feedback__item">
        <ds-about/>
      </div>
    </div>
  </div>
</template>

<script>
import DsAbout from "@/components/home/dsAbout"

export default {
  name: "dsFeedback",
  components: {
    DsAbout
  }
}
</script>