<template>
  <v-app>
    <v-main>
      <NavMenu />
      <v-container>
        <nuxt />
      </v-container>
      <Footer />
    </v-main>
  </v-app>
</template>

<script>
export default {

}
</script>
<style scoped>
a {
  text-decoration: none;
  color: black;
}
a:hover {
  text-decoration: none;
  color: black;
}
.section {
  margin: 3em 0;
}
.center {
  display: flex;
  flex-direction: row;
  justify-content: center;
}
.text-medium {
  font-weight: 400;
}

.text-bold {
  font-weight: 700;
}
.button-custom {
  font-family: 'Montserrat';
}
.flex {
  display: flex;
  flex-direction: row;
}

.flex-row {
  justify-content: space-between;
}

.flex-vertical {
  display: flex;
  flex-direction: column;
}

.main-container {
  padding: 0 120px;
}

.nav-containter {
  height: 30px;
}
* {
  font-family: 'Montserrat';
}
</style>
