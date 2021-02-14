<template>
  <div>
    <v-app-bar style="background-color: #05aff2;" dense>
      <v-container>
        <v-row style="text-align: start;">
          <v-col sm="3" md="2" lg="2">
            <v-toolbar-title
              style="color: white; font-family: Montserrat; font-weight: bold;"
              >FCoarcaDent</v-toolbar-title
            >
          </v-col>
          <v-spacer></v-spacer>
          <v-col
            v-if="$vuetify.breakpoint.smAndUp"
            style="text-align: end; font-family: Montserrat; font-weight: thin;"
            sm="9"
            md="10"
            lg="10"
          >
            <a
              class="pa-2"
              :class="{
                'mr-5': $vuetify.breakpoint.mdAndUp,
                'mr-3': $vuetify.breakpoint.sm
              }"
              style="color: white;"
              href="#"
              >Despre</a
            >

            <a
              class="pa-2"
              :class="{
                'mr-5': $vuetify.breakpoint.mdAndUp,
                'mr-3': $vuetify.breakpoint.sm
              }"
              style="color: white;"
              href="#"
              >Servicii Stomatologice</a
            >

            <a
              class="pa-2"
              :class="{
                'mr-5': $vuetify.breakpoint.mdAndUp,
                'mr-3': $vuetify.breakpoint.sm
              }"
              style="color: white;"
              href="/preturi"
              >Preturi</a
            >

            <a
              style="
                background-color: #f2b705;
                border-radius: 25px;
                text-align: center;
              "
              class="px-3"
              href="#"
              >Contact</a
            >
          </v-col>
          <v-col v-if="$vuetify.breakpoint.xsOnly" cols="2">
            <v-app-bar-nav-icon
              @click.stop="drawer = !drawer"
            ></v-app-bar-nav-icon>
          </v-col>
          <v-navigation-drawer
            v-model="drawer"
            style="background-color: #028cc2;"
            right
            absolute
            app
            temporary
          >
            <v-list nav dense>
              <v-list-item-group>
                <v-list-item>
                  <v-list-item-title
                    style="color: white; font-family: Montserrat;"
                    >Despre</v-list-item-title
                  >
                </v-list-item>

                <v-list-item>
                  <v-list-item-title
                    style="color: white; font-family: Montserrat;"
                    >Servicii Stomatologice</v-list-item-title
                  >
                </v-list-item>

                <v-list-item>
                  <v-list-item-title
                    style="color: white; font-family: Montserrat;"
                    >Preturi</v-list-item-title
                  >
                </v-list-item>

                <v-list-item>
                  <v-list-item-title
                    style="color: white; font-family: Montserrat;"
                    >Contact</v-list-item-title
                  >
                </v-list-item>
              </v-list-item-group>
            </v-list>
          </v-navigation-drawer>
        </v-row>
      </v-container>
    </v-app-bar>
  </div>
  <!-- <div class="container-fluid blue flex flex-row nav-container">
    <div class="logo">
      <h1 class="h1">FCoarcaDent</h1>
    </div>
    <div class="menu">
      <ul class="nav w-100 justify-content-end">
        <li class="nav-item">
          <a class="nav-link active" href="#">Despre</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Servicii Stomatologice</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="/preturi">Preturi</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Contact</a>
        </li>
      </ul>
    </div>
  </div> -->
</template>
<script>
export default {
  name: 'NavMenu',
  data: () => ({
    drawer: false
  })
}
</script>
<style>
/* .nav {
  height: 50px;
}

.logo h1 {
  color: white;
} */
</style>
