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
    <div class="row">
      <ds-sidebar/>
    </div>
  </div>
</template>

<script>
import DsBreadcrumbs from "@/components/app/dsBreadcrumbs"
import DsSidebar from "@/components/catalog/dsSidebar"

export default {
  name: 'Catalog',
  components: {
    DsSidebar,
    DsBreadcrumbs
  }
}
</script>
