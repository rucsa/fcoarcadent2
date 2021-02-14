<template>
  <div>
    <h3>{{ cardTitle }}</h3>
    <div v-for="item in cardContent" :key="item.service">
      <PriceItem :service="item.service" :price="item.price" />
    </div>
  </div>
</template>
<script>
export default {
  name: 'PriceCard',
  props: {
    cardTitle: {
      type: String,
      default: ''
    },
    cardContent: {
      type: Array,
      default: null
    }
  }
}
</script>
