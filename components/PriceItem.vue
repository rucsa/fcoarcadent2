<template>
  <div class="flex wrap-row">
    <p>{{ service }}</p>
    <p>{{ price }}</p>
  </div>
</template>
<script>
export default {
  name: 'PriceItem',
  props: {
    service: {
      type: String,
      default: ''
    },
    price: {
      type: String,
      default: ''
    }
  }
}
</script>
<style scoped>
.wrap-row {
  justify-content: space-between;
}

p {
  font-size: 1.3em;
}
</style>
