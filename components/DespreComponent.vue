<template>
  <div class="container">
    <h1 class="center">Despre Noi</h1>
    <div class="flex">
      <div class="about-intro-img"></div>
      <div class="flex-vertical">
        <div class="about-intro-text">
          <p>
            {{ aboutUsText1 }}
          </p>
          <p>
            {{ aboutUsText2 }}
          </p>
          <blockquote>
            <h3 class="special-text">
              {{ specialText }}
            </h3>
          </blockquote>
        </div>
        <div class="flex center-items center">
          <Button button-title="Citeste mai multe" to="/about/" />
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import Button from '~/components/Button.vue'

export default {
  name: 'DespreComponent',
  components: { Button },
  data() {
    return {
      aboutUsText1:
        'Misiunea unui doctor stomatolog este să readuca în viața pacienților săi placerea și dorința de a-și trăi viața la cele mai înalte standarde.',
      aboutUsText2:
        'Un zâmbet pe fața pacientului este confirmarea că ne-am îndeplinit angajamentele luate prin',
      specialText: 'Jurământul lui Hippocrate'
    }
  },
  computed: {
    owner() {
      return {}
    }
  },
  methods: {}
}
</script>

<style scoped>
.about-intro-text p {
  font-family: HindSiliguri;
  font-family: 20px;
}

.about-intro-img {
  width: 60vw;
  height: 300px;
  display: block;
  background-image: url('./../assets/img/DSC_0160.jpg');
  background-size: cover;
  background-repeat: no-repeat;
}

.about-intro-text {
  padding: 1vh 5vw;
}
</style>
