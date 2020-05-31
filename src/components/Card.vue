<template>
  <v-row
  >
    <v-col
      v-for="item in items"
      md="4"
      sm="6"
      xs="12"
      :key="item"
    >

    <v-card
      max-width="344"
      class="mx-auto"
    >
      <v-img
        :src="item.thumbnailUrl"
        height="194"
      ></v-img>

      <v-card-title>{{item.title}}</v-card-title>
      <v-card-subtitle>東海オンエア</v-card-subtitle>
      <v-card-text>
        Visit ten places on our planet that are undergoing the biggest changes today.
      </v-card-text>

      <v-card-actions>
        <v-btn
          text
          color=""
        >
          Read
        </v-btn>
        <v-btn
          text
          color=""
        >
          Bookmark
        </v-btn>
        <v-spacer></v-spacer>
        <v-btn icon>
          <v-icon>mdi-heart</v-icon>
        </v-btn>
        <v-btn icon>
          <v-icon>mdi-share-variant</v-icon>
        </v-btn>
      </v-card-actions>
    </v-card>
  </v-col>
</v-row>

</template>
<script>
  export default {
  data:() => ({
    parentMessage: 'Parent',
    items: [
      {
        "id": 1,
        "title": "【大貸切】真夜中のイオンモールで警備員から逃げながら隠された私物を探し出せ！！",
        "thumbnailUrl": "https://i.ytimg.com/vi/jpqfA6Om_dM/default.jpg",
        "likeCount": "6424",
        "dislikeCount": "92"
      },
      {
        "id": 2,
        "title": "【精神破壊】これ、どれが本当のアンチコメ？",
        "thumbnailUrl": "https://i.ytimg.com/vi/FoWDMUUlRG4/default.jpg",
        "likeCount": "6424",
        "dislikeCount": "92"
      },
      {
        "id": 3,
        "title": "【近未来】セグウェイ乗ってスポーツやったら何でも新競技じゃね？",
        "thumbnailUrl": "https://i.ytimg.com/vi/h1Bwmire0sg/default.jpg",
        "likeCount": "6424",
        "dislikeCount": "92"
      },
      {
        "id": 4,
        "title": "1万円でたくさん買い物した方が勝ち対決！",
        "thumbnailUrl": "https://i.ytimg.com/vi/oQj91piFKjo/default.jpg",
        "likeCount": "6424",
        "dislikeCount": "92"
      },
      {
        "id": 5,
        "title": "東海オンエアの中で1番多く｢動画の中でボケてる奴｣って誰なんだ？",
        "thumbnailUrl": "https://i.ytimg.com/vi/5W1e6p7dPnk/default.jpg",
        "likeCount": "6424",
        "dislikeCount": "92"
      },
      {
        "id": 6,
        "title": "【負けたらウォーリー】映像の中に隠れているてつやを探せ！！！",
        "thumbnailUrl": "https://i.ytimg.com/vi/7OoGuwL5-Q8/default.jpg",
        "likeCount": "6424",
        "dislikeCount": "92"
      }
    ]
  })
  }
</script>