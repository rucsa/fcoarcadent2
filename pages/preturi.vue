<template>
  <div class="">
    <h1 class="">Prețuri</h1>
    <ul>
      <li v-for="item in myJson" :key="item.title">
        <PriceCard :card-title="item.title" :card-content="item.content" />
      </li>
    </ul>
  </div>
</template>
<script>
import prices from '~/assets/data/preturi.json'
export default {
  metaInfo: {
    title: 'About us'
  },
  data() {
    return {
      myJson: prices
    }
  }
}
</script>
