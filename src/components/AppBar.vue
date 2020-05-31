<template>
  <v-app-bar
    app
    clipped-left
    color="red"
    dense
  >
    <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
    <v-icon
      class="mx-4"
      large
    >
      mdi-youtube
    </v-icon>
    <v-toolbar-title class="mr-12 align-center">
      <span 
      class="title"
      style="color:white;"
      >Youtube</span>
    </v-toolbar-title>
    <v-spacer></v-spacer>
    <v-row
      align="center"
      style="max-width: 240px"
    >
      <v-text-field
        :append-icon-cb="() => {}"
        placeholder="  キーワードを入力"
        single-line
        append-icon="mdi-magnify"
        color="white"
        hide-details
        background-color="white"
      ></v-text-field>
    </v-row>
  </v-app-bar>
</template>

<script>
  export default {
    data: () => ({
      drawer: null
    })
  }
</script>