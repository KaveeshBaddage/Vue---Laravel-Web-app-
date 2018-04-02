<template>
<v-list class="pt-0" dense>
    <v-divider></v-divider>
        <v-list-tile>
            <v-list-tile-content>
              <v-list-tile-title><h1><b>Tesseract OCR</b></h1></v-list-tile-title>
            </v-list-tile-content>
          </v-list-tile>
           <v-divider></v-divider>
        <v-list-tile v-for='item in items' :key='item.title' @click='1'>
          <v-list-tile-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>{{ item.title }}</v-list-tile-title>
          </v-list-tile-content>
     </v-list-tile>
</v-list>
</template>

<script>
export default {
  data: () => ({
    items: [
      { title: 'Home', icon: 'dashboard' },
      { title: 'About', icon: 'question_answer' },
      { title: 'Contact Us', icon: 'contact_mail' }
    ]
  }
  )
}
</script>

<style scoped>
</style>
