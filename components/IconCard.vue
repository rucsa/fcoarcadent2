<template>
  <div class="card centered-text square-shadow">
    <div class="">
      <p>TODO: add icon from {{ imagesrc }}</p>
      <p>{{ cardText }}</p>
    </div>
  </div>
</template>
<script>
export default {
  name: 'IconCard',
  props: {
    imagesrc: {
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
  background-color: grey;
}
</style>
