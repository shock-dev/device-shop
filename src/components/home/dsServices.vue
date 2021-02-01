<template>
  <div class="services">
    <div class="container">
      <div class="services__inner">
        <div class="services__tabs-box">
          <button
            class="services__tab"
            v-for="tab in tabs"
            :key="tab.id"
            :class="{ active: tab.id === activeTab }"
            @click="activeTab = tab.id"
          >{{ tab.title }}</button>
        </div>
        <div class="services__content">
          <div class="services__content-item">
            <div class="services__content-info">
              <div class="services__content-title">Доставка</div>
              <p class="services__content-text">
                Мы с удовольствием доставим ваш товар прямо к вашему подъезду совершенно бесплатно! Ведь мы неплохо заработаем, поднимая его на ваш этаж.
              </p>
            </div>
            <img src="~@/assets/img/delivery-image.png" alt="Delivery">
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "dsServices",
  data: () => ({
    tabs: [
      {
        id: 1,
        title: 'Доставка'
      },
      {
        id: 2,
        title: 'Гарантия'
      },
      {
        id: 3,
        title: 'Кредит'
      }
    ],
    activeTab: 0
  })
}
</script>