<template>
  <v-content>
    <v-container 
    class="fill-height"
    style="background-color:#fcfcfc;"
    >
      <!-- ヘッダー画像 -->
      <v-row
        justify="center"
        align="center"
      >       
        <v-img
          src="https://yt3.ggpht.com/Axwfv08O1e7Bv0uhjh0msKuadvKZhWkzeEilVCCDVqonymJNjhW1GmnNTWzzlEoY4IoeUGB_nQ=w1060-fcrop64=1,00005a57ffffa5a8-k-c0xffffffff-no-nd-rj"
          height="194"
        ></v-img>
      </v-row>

      <!-- チャンネルアイコン -->
      <v-row
        justify="center"
        align="center"
      >
        <v-col
          cols="auto"
          style="margin-left:50px;"
        >
          <v-avatar color="orange" size="80">
            <img
              src="https://yt3.ggpht.com/a/AATXAJyL85STIntBttIC1v57dKa9sqybrq2_xfBRIw=s240-c-k-c0xffffffff-no-rj-mo"
              alt=""
            >
          </v-avatar>
        </v-col>
        <v-col>
          <v-list
          style="padding:0; background-color:#fcfcfc;">
            <v-list-item
            style="padding:0;">
              <v-list-item-content>
                <v-list-item-title class="" style="font-size: 24px;">東海オンエア</v-list-item-title>
                <v-list-item-subtitle>チャンネル登録者数XX人</v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
          </v-list>
        </v-col>
        <v-col
        cols="auto"
          >
          <v-btn color="error">Error</v-btn>
        </v-col>
      </v-row>

      <v-tabs v-model="model">
        <v-tab href="#test1">
          ホーム
        </v-tab>
        <v-tab href="#test2">
          動画
        </v-tab>
        <v-tab href="#test3">
          XXX
        </v-tab>
      </v-tabs>

      <v-tabs-items v-model="model" fixed-tabs="true">
        <v-tab-item value="test1">
          <!-- 動画 -->
          <v-row>
            <v-col>
              アップロード動画
            </v-col>
          </v-row>
          <Card/>
        </v-tab-item>
        <v-tab-item value="test2">
          test
        </v-tab-item>
      </v-tabs-items>




      <!-- 不要 -->
      <v-row
        justify="center"
        align="center"
      >
        <v-col class="shrink">
          <v-tooltip right>
            <template v-slot:activator="{ on }">
              <v-btn
                :href="source"
                icon
                large
                target="_blank"
                v-on="on"
              >
                <v-icon large>mdi-code-tags</v-icon>
              </v-btn>
            </template>
            <span>Source</span>
          </v-tooltip>
        </v-col>
      </v-row>
    </v-container>
  </v-content>
</template>

<script>
import Card from './Card';

  export default {
    components: {
      Card
    },
    props: {
      source: String,
    },
    data () {
      return {
        model: 'tab-1'
    }
  }
  }
</script>