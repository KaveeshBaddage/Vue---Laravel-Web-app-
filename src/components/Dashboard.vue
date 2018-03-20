<template>
<div id="app">
  <v-app id="inspire">
   <v-navigation-drawer
      fixed
      v-model="drawer"
      app
    >
      <v-list dense>
        <v-list-tile @click="">
          <v-list-tile-action>
            <v-icon>home</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>Home</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile @click="">
          <v-list-tile-action>
            <v-icon>home</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>Get Text</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile @click="">
          <v-list-tile-action>
            <v-icon>contact_mail</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>Contact Us</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
        <v-toolbar color="dark grey" dark fixed app>
      <v-toolbar-side-icon @click.stop="drawer = !drawer"></v-toolbar-side-icon>
      <v-toolbar-title>Tesseract OCR</v-toolbar-title>
    </v-toolbar>
    <v-content>
               <v-jumbotron color="">
                <v-container fill-height>
                  <v-layout align-center>
                    <v-flex>
                      <h3 class="display-3">Welcome to the Tesseract OCR</h3>
                      <span class="subheading"> Free Online OCR service allows you to convert scanned images to editable text formats and extract text from JPEG/TIFF/BMP files.</span>
                      <v-divider class="my-3"></v-divider>
                      <div class="title mb-3">Check out our newest features!</div>
                      <v-btn large color="primary" class="mx-0">See more</v-btn>
                    </v-flex>
                  </v-layout>
                </v-container>
              </v-jumbotron>
    </v-content>
    <v-footer app>
          <v-spacer></v-spacer>
          &copy; Kaveesh Baddage
    </v-footer>
  </v-app>
</div>

</template>

<script>
export default {
  name: "Dashboard",
  data() {
    return {
      data: "dashboard data",
      drawer: null
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}
a {
  color: #42b983;
}
</style>
