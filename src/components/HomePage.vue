<template>
<v-jumbotron color="">
    <v-container fill-height>
      <v-layout align-center>
        <v-flex>
          <h3 class="display-3">Welcome to the Tesseract OCR</h3>
          <span class="subheading"> Free Online OCR service allows you to convert scanned images to editable text formats and extract text from JPEG/TIFF/BMP files.</span>
          <v-divider class="my-3"></v-divider>
          <div class="title mb-3">Check out our newest features!</div>
          <v-btn  @click="drawer = !drawer" large color="primary" class="mx-0">See more</v-btn>
        </v-flex>
     </v-layout>
    </v-container>
  </v-jumbotron>
</template>

<script>
export default {
  data: () => ({
    drawer: false
  }
  )
}
</script>

<style scoped>
</style>
