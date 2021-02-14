<template>
  <v-footer color="#05AFF2" padless>
    <v-container>
      <v-row justify="center">
        <v-col cols="12" sm="9" md="9" lg="9" :align="changeAlign()">
          <a
            class="pa-2"
            :class="{
              'mr-5': $vuetify.breakpoint.smAndUp,
              'mr-8': $vuetify.breakpoint.xsOnly
            }"
            style="color: white;"
            href="#"
            >Despre</a
          >

          <a
            class="pa-2"
            :class="{
              'mr-5': $vuetify.breakpoint.smAndUp,
              'mx-6': $vuetify.breakpoint.xsOnly
            }"
            style="color: white;"
            href="#"
            >Preturi</a
          >

          <a
            style="color: white;"
            class="pa-2"
            :class="{
              'mr-5': $vuetify.breakpoint.smAndUp,
              'ml-8': $vuetify.breakpoint.xsOnly
            }"
            href="/preturi"
            >Servicii</a
          >
        </v-col>
        <v-col
          v-if="$vuetify.breakpoint.smAndUp"
          style="text-align: end;"
          sm="3"
          md="3"
          lg="3"
        >
          <v-spacer> </v-spacer>

          <div>
            <p class="font-weight-bold">{{ actionText }}</p>
          </div>
        </v-col>
        <v-col class="py-4 text-center" cols="12">
          <div style="color: white;">
            {{ copyrights }}
          </div>
        </v-col>
      </v-row>
    </v-container>
  </v-footer>
</template>
<script>
export default {
  name: 'Footer',
  data() {
    return {
      alignChang: 'start',
      copyrights:
        '@2020 Cabinet Stomatologic Filofteia Coarca | Created by Vulpix',
      actionText: '+4 0724 545 168',
      links: ['Despre', 'Preturi', 'Servicii']
    }
  },
  // eslint-disable-next-line object-shorthand
  methods: {
    changeAlign() {
      if (this.$vuetify.breakpoint.xsOnly) {
        return 'center'
      } else {
        return 'start'
      }
    }
  }
}
</script>
<style scoped>
/* .footer {
  height: 123px;
} */
* {
  font-family: Montserrat;
  color: white;
}
</style>
