<template>
  <v-container>
    <span class="red--text">Class works!</span>
    <Cover />
        <DespreComponent />
    <Servicii />
    <Contact />
  </v-container>
</template>

<script>
export default {
  data() {
      return {
        title: 'Cabinet Stomatologic dr. Filofteia Coarca'
      }
    },
    head() {
    return {
      title: this.title,
      meta: [
        {
          hid: 'fcoarcadent',
          name: 'Cabinet Stomatologic dr. Filofteia Coarca',
          content: 'Cabinet Stomatologic situat in Sector 1 Bucuresti'
        }
      ]
    }
  }
}
</script>
