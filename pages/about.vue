<template>
  <div class="">
    <div class="">
      <div class="">
        <p>Medic titular: {{ name }}</p>
        <p>Grad medical: {{ grad }}</p>
        <p>Experiență: {{ experienta }}</p>
        <p>Perfecționare profesională: {{ perfectionare }}</p>
        <p>Atitudine: {{ atitudine }}</p>
        <h3 class="">{{ specialtext }}</h3>
      </div>
      <div class="about-intro-img"></div>
    </div>
    <div>
      <div class="">
        <div class="">
          <IconCard
            imagesrc="~/assets/icons/1.png"
            card-text="Profesionalismul si dedicatia personalului medical"
          />
          <IconCard
            imagesrc="~/assets/icons/2.png"
            card-text="Aparatura medicala stomatologica de ultima generatie"
          />
          <IconCard
            imagesrc="~/assets/icons/3.png"
            card-text="Tehnici medicale stomatologice inovatoare"
          />
          <IconCard
            imagesrc="~/assets/icons/4.png"
            card-text="Adresabilitate maxima corespunzatoare cerințelor pacienților"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'About',
  data() {
    return {
      name: 'Coarcă Filofteia',
      grad: 'Medic stomatolog specialist',
      experienta:
        '33 ani vechime și peste 10.000 de pacienți tratati cu succes',
      perfectionare:
        'Continuă prin participare la congrese, simpozioane, workshopuri, cursuri de perfecționare în stomatologie',
      atitudine: 'Hotărîre, perseverență, apropiat și înțelegător cu pacienții',
      specialtext: 'Apreciată de micii pacienti'
    }
  },
  computed: {
    owner() {
      return {
        name: 'Filofteia Coarca'
      }
    }
  },
  methods: {}
}
</script>

<style scoped>
.about-intro-img {
  width: 900px;
  height: 350px;
  padding: 0 0 0 5vw;
  box-shadow: 3px 3px 5px grey;
  background-image: url('./../assets/DSC_0206.jpg');
  background-repeat: no-repeat;
}
</style>
