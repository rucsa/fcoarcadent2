<template>
  <div class="card">
    <div class="">
      <h3>{{ cardTitle }}</h3>
    </div>
  </div>
</template>
<script>
export default {
  name: 'Card',
  props: {
    cardTitle: {
      type: String,
      default: ''
    },
    cardText: {
      type: String,
      default: ''
    }
  }
}
</script>
<style scoped>
.card {
  margin: 1em;
  height: 10em;
  width: 15em;
}
</style>
