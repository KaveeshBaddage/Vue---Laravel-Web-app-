<template>
<div id="app">
  <v-app id="inspire">
   <v-navigation-drawer
      fixed
      v-model="drawer"
      app
    ><sidebar></sidebar>
    </v-navigation-drawer>
        <v-toolbar color="dark grey" dark fixed app>
      <v-toolbar-side-icon @click.stop="drawer = !drawer"></v-toolbar-side-icon>
      <v-toolbar-title>Tesseract OCR</v-toolbar-title>
    </v-toolbar>
    <v-content>
  <homePage :parentData="parentData"></homePage>
  </v-content>
  <customFooter></customFooter>
  </v-app>
</div>
</template>

<script>
import sidebar from './Sidebar.vue'
import customFooter from './Footer.vue'
import homePage from './HomePage.vue'
export default {
  name: 'Dashboard',
  data: () => ({
    drawer: false,
    parentData: true
  }
  ),
  components: {
    sidebar,
    customFooter,
    homePage
  },
  method: {
    handleFcAfterDateBack: function (event) {
      console.log('data after child handle: ', event) // get the data after child dealing
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal
}
a {
  color: #42b983
}
</style>
