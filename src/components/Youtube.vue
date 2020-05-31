<template>
  <v-content>
    <v-container 
    class="fill-height"
    style="background-color:#fcfcfc;"
    >
      <v-row
        justify="center"
        align="center"
      >       
        <v-img
          src="https://yt3.ggpht.com/Axwfv08O1e7Bv0uhjh0msKuadvKZhWkzeEilVCCDVqonymJNjhW1GmnNTWzzlEoY4IoeUGB_nQ=w1060-fcrop64=1,00005a57ffffa5a8-k-c0xffffffff-no-nd-rj"
          height="194"
        ></v-img>
      </v-row>

      <v-row
        justify="center"
        align="end"
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
                <v-list-item-title class="" style="font-size: 24px; font-weight:bold;">東海オンエア</v-list-item-title>
                <v-list-item-subtitle>チャンネル登録者数XX人</v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
          </v-list>

        </v-col>
      </v-row>


      <Card/>
      <!-- <v-row
        justify="start"
        align="start"
      >
      <v-col>
        <Card/>
      </v-col>
      </v-row> -->

      <!-- <v-row
        justify="start"
        align="start"
      >
        <Card/>
        <Card/>
        <Card/>
      </v-row> -->

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
    }
  }
</script>