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
          <div
            class="services__content-item"
            v-for="item in content"
            :key="item.id"
            :class="{ hide: activeTab !== item.id }"
          >
            <div class="services__content-info">
              <div class="services__content-title">{{ item.title }}</div>
              <p class="services__content-text">
                {{ item.text }}
              </p>
            </div>
            <img :src="item.imageUrl" :alt="item.title">
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
    activeTab: 1,
    content: [
      {
        id: 1,
        title: 'Доставка',
        text: 'Мы с удовольствием доставим ваш товар прямо к вашему подъезду совершенно бесплатно! Ведь мы неплохо заработаем, поднимая его на ваш этаж.',
        imageUrl: require('@/assets/img/delivery-image.png')
      },
      {
        id: 2,
        title: 'Гарантия',
        text: 'Мы с удовольствием доставим ваш товар прямо к вашему подъезду совершенно бесплатно! Ведь мы неплохо заработаем, поднимая его на ваш этаж.',
        imageUrl: require('@/assets/img/delivery-image.png')
      },
      {
        id: 3,
        title: 'Кредит',
        text: 'Мы с удовольствием доставим ваш товар прямо к вашему подъезду совершенно бесплатно! Ведь мы неплохо заработаем, поднимая его на ваш этаж.',
        imageUrl: require('@/assets/img/delivery-image.png')
      }
    ]
  })
}
</script>