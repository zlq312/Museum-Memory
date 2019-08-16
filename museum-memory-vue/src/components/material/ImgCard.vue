<template>
    <v-card class="mx-auto" 
    >
        <v-img class="white--text" height="200px" :src="url">
            <v-card-title class="align-end fill-height">{{ title }}</v-card-title>
        </v-img>
        <v-card-text>{{ text }}</v-card-text>
        <v-card-actions v-if="actions">
            <v-btn icon>
                <v-icon>mdi-heart</v-icon>
            </v-btn>
            <v-btn text>Click</v-btn>
            <v-btn outlined>Click</v-btn>
        </v-card-actions>
    </v-card>
</template>
<script>
export default {
    inheritAttrs: false,

    props: {
      url: {
        type: String,
        default: undefined
      },
      actions: {
        type: Boolean,
        default: false
      },
      title: {
        type: String,
        default: "Title"
      },
      text: {
        type: String,
        default: "Content"
      }
    }
}
</script>