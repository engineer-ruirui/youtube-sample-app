<template>
  <v-navigation-drawer
    v-model="drawer"
    app
    clipped
  >
    <v-list dense>
      <v-list-item
        v-for="item in items"
        :key="item.text"
        link
      >
        <v-list-item-action>
          <v-icon>{{ item.icon }}</v-icon>
        </v-list-item-action>
        <v-list-item-content>
          <v-list-item-title>
            {{ item.text }}
          </v-list-item-title>
        </v-list-item-content>
      </v-list-item>
      <v-subheader class="mt-4 grey--text text--darken-1">登録チャンネル</v-subheader>
      <v-list>
        <v-list-item
          v-for="item in items2"
          :key="item.text"
          link
        >
          <v-list-item-avatar>
            <img
              :src="`${item.picture}`"
              alt=""
            >
          </v-list-item-avatar>
          <v-list-item-title v-text="item.text"></v-list-item-title>
        </v-list-item>
      </v-list>
      <v-list-item
        class="mt-4"
        link
      >
        <v-list-item-action>
          <v-icon color="grey darken-1">mdi-plus-circle-outline</v-icon>
        </v-list-item-action>
        <v-list-item-title class="grey--text text--darken-1">Browse Channels</v-list-item-title>
      </v-list-item>
      <v-list-item link>
        <v-list-item-action>
          <v-icon color="grey darken-1">mdi-cog</v-icon>
        </v-list-item-action>
        <v-list-item-title class="grey--text text--darken-1">Manage Subscriptions</v-list-item-title>
      </v-list-item>
    </v-list>
  </v-navigation-drawer>
</template>

<script>
  export default {
    props: {
      source: String,
    },
    data: () => ({
      drawer: null,
      items: [
        { icon: 'mdi-trending-up', text: 'Most Popular' },
        { icon: 'mdi-youtube-subscription', text: 'Subscriptions' },
        { icon: 'mdi-history', text: 'History' },
        { icon: 'mdi-playlist-play', text: 'Playlists' },
        { icon: 'mdi-clock', text: 'Watch Later' },
      ],
      items2: [
        { picture: 'https://yt3.ggpht.com/a/AATXAJyL85STIntBttIC1v57dKa9sqybrq2_xfBRIw=s240-c-k-c0xffffffff-no-rj-mo', text: '東海オンエア' },
        { picture: 38, text: '東海オンエア' },
        { picture: 48, text: 'Xbox Ahoy' },
        { picture: 58, text: 'Nokia' },
        { picture: 78, text: 'MKBHD' },
      ],
    })
  }
</script>