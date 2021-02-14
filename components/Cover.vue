<template>
  <!-- <div> -->
  <!-- <v-container class="px-0 py-0" fluid> -->
  <!-- <v-row>
      <v-col> -->
  <!-- <v-card flat tile> -->
  <v-img height="702px" :src="require(`./../assets/LPPhoto.png`)">
    <v-card-text style="text-align: start;">
      <h2>{{ title }}</h2>
      <h2>{{ title2 }}</h2>
      <h3>
        <span class="text-medium">Lucrăm cu oameni </span><br /><span
          class="text-bold"
          >și pentru oameni</span
        >
      </h3>
    </v-card-text>
  </v-img>
  <!-- </v-card> -->
  <!-- </v-col>
    </v-row> -->
  <!-- </v-container> -->
  <!-- </div> -->
  <!-- <div class="cover">
    <div class="cover-content">
      <div class="cover-text">
        <h1 class="h1 anada">{{ title }}</h1>
        <h1 class="h1">
          <span class="monser">{{ title2 }}</span>
        </h1>
        <h3 class="h3">
          <span class="text-medium">Lucrăm cu oameni </span><br /><span
            class="text-bold"
            >și pentru oameni</span
          >
        </h3>
      </div>
      <div class="cover-buttons flex center-items center">
        <Button button-title="Despre noi" to="#" />
        <Button button-title="Contact" to="#" />
      </div>
    </div>
  </div> -->
</template>
<script>
// import Button from '~/components/Button.vue'

export default {
  name: 'Cover',
  // components: { Button },
  data() {
    return {
      title: 'Cabinet Stomatologic',
      title2: 'dr. Filofteia Coarcă'
    }
  }
}
</script>
<style scoped>
/* h1,
.anada {
  font-family: 'Ananda';
}

h2,
.monser {
  font-family: 'Montserrat';
}

.cover {
  background-image: url('./../assets/LPPhoto.png');
  background-repeat: no-repeat;
  background-size: contain;
  max-width: 100vw;
  height: 702px;
  border: 1px solid black;
}
.cover-content {
  position: relative;
  top: 10em;
  left: 6em;
  width: 25em;
  height: 20em;
  border: 1px solid black;
} */
</style>
