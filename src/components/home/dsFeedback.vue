<template>
  <div class="container">
    <div class="row feedback">
      <div class="col-50 feedback__item">
        <ds-about/>
      </div>
      <div class="col-50 feedback__item">
        <ds-contacts/>
      </div>
    </div>
  </div>
</template>

<script>
import DsAbout from "@/components/home/dsAbout"
import DsContacts from "@/components/home/dsContacts"

export default {
  name: "dsFeedback",
  components: {
    DsContacts,
    DsAbout
  }
}
</script>