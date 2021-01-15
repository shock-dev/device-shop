<template>
  <div id="app">
    <ds-header/>
    <router-view/>
  </div>
</template>

<style lang="scss">
@import "~@/scss/index.scss";
</style>
<script>
import DsHeader from "@/components/app/dsHeader";

export default {
  components: {
    DsHeader
  }
}
</script>
