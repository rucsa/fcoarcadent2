<template>
  <div class="button-custom">
    <a :href="to">{{ buttonTitle }}</a>
  </div>
</template>
<script>
export default {
  name: 'Button',
  props: {
    anchor: {
      type: Boolean,
      required: false,
      default: false
    },
    buttonTitle: {
      type: String,
      default: ''
    },
    to: {
      type: String,
      default: ''
    },
    fontSize: {
      type: Number,
      default: 30
    },
    fontWeigth: {
      type: Number,
      default: 800
    }
  }
}
</script>
<style scoped>
a {
  font-family: 'Montserrat';
  padding: 0.5em 2.5em;
  font-size: 0.8em;
  font-weight: 800;
  background: #f2b705 0% 0% no-repeat padding-box;
  border-radius: 15px;
  opacity: 1;
}
</style>
