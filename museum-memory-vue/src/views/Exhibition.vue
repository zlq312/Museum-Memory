<template>
  <v-container
    fill-height
    fluid
    grid-list-xl
  >
    <v-layout wrap>
      <v-flex
        md12
        sm12
        lg4

         v-for="exhibition in exhibitions"
      >

        <material-img-card
          :url="exhibition.url"
          :text="exhibition.desc"
          :title="exhibition.name"
        >
        </material-img-card>

      </v-flex>
   
     
    </v-layout>
  </v-container>
</template>

<script>
export default {
  data () {
    return {
      exhibitions: [
        {
          name: "fangao",
          desc: "first",
          url : 'https://cdn.vuetifyjs.com/images/cards/docks.jpg'
        },
        {
          name: "monai",
          desc: "second",
          url : 'https://cdn.vuetifyjs.com/images/cards/docks.jpg'
        },
        {
          name: "fangao2",
          desc: "first2",
          url : 'https://cdn.vuetifyjs.com/images/cards/docks.jpg'
        },
        {
          name: "fangao3",
          desc: "first3",
          url : 'https://cdn.vuetifyjs.com/images/cards/docks.jpg'
        }
      ]
    }
  }
}
</script>
