<template>
  <v-app>
    <!-- ヘッダー -->
    <AppBar/>
    <!-- ナビゲーションバー -->
    <NavigationDrawer/>
    <!-- <v-content> -->
      <Youtube/>
    <!-- </v-content> -->
  </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld';
import NavigationDrawer from './components/NavigationDrawer';
import Youtube from './components/Youtube';
import AppBar from './components/AppBar';

export default {
  name: 'App',

  components: {
    // HelloWorld,
    NavigationDrawer,
    Youtube,
    AppBar
  },
  data: () => ({
    //
  }),
  created () {
    // this.$vuetify.theme.dark = true
  }

};
</script>
