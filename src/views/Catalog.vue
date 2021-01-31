<template>
  <div class="catalog">
    <div class="container">
      <div class="catalog__inner">
        <div class="catalog__head">
          <h2 class="catalog__title">Моноподы для селфи</h2>
        </div>
        <ds-breadcrumbs/>
      </div>
    </div>
  </div>
</template>

<script>
import DsBreadcrumbs from "@/components/app/dsBreadcrumbs"

export default {
  name: 'Catalog',
  components: {
    DsBreadcrumbs
  }
}
</script>
