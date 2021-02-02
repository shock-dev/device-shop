<template>
  <div id="app">
    <ds-header/>
    <router-view/>
    <ds-footer/>
  </div>
</template>

<style lang="scss">
@import "~@/scss/index.scss";
</style>
<script>
import DsHeader from "@/components/app/dsHeader"
import DsFooter from "@/components/app/dsFooter"

export default {
  components: {
    DsFooter,
    DsHeader
  }
}
</script>
