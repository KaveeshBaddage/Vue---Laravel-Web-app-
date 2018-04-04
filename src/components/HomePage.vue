<template>
<v-jumbotron color="">
    <v-container fill-height>
      <v-layout align-center>
        <v-flex>
          <h3 class="display-3">Welcome to the Tesseract OCR</h3>
          <span class="subheading"> Free Online OCR service allows you to convert scanned images to editable text formats and extract text from JPEG/TIFF/BMP files.</span>
          <v-divider class="my-3"></v-divider>
          <div class="title mb-3">Check out our newest features!</div>
          <v-btn  @click="counter += 1,childData = !childData" large color="primary" class="mx-0">See more</v-btn>
          <p>The button above has been clicked {{ counter }} {{ drawer }} {{childData}} times.</p>
        </v-flex>
     </v-layout>
    </v-container>
  </v-jumbotron>
</template>

<script>
export default {
  data: () => ({
    drawer: false,
    counter: 0,
    childData: ''
  }
  ),
  props: {
    parentData: {
      type: Boolean,
      default () {
        return true
      }
    }
  },
  methods: {
    // maybe onchagne may onclick whatever..
    // handleDataFc: function () {
    //   this.$emit('interface', this.childData) // handle data and give it back to parent by interface
    // }
  },
  beforeMount () {
    this.childData = this.parentData // save props data to itself's data and deal with it
  }
}
</script>

<style scoped>
</style>
