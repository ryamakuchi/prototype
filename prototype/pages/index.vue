<template>
  <v-app id="home my-3">
    <div class="box" id="hero">
      <div class="hero">物語との出会いを通して、人類に感動する機会を提供する</div>
    </div>
    <section>
      <v-layout
        column
        wrap
        class="my-5"
        align-center
        text-xs-center
      >

      <div class="product">
          <v-flex xs12 class="my-3">
            <h1 class="headline">プロダクト</h1>
            <span class="subheading">国内最大級の映画・ドラマ・アニメの情報サービスciatr[シアター]の企画・開発・運営を行っています。</span>
            <v-flex xs8 offset-xs2 class="my-5">
              <v-jumbotron color="white lighten-2" class="elevation-3" height="auto">
                <v-container grid-list-xl>
                  <v-layout row wrap align-center>
                    <v-flex xs12 md6 justify-space-around>
                      <img src="../assets/ciatr.jpg" alt="ciatr" style="width:100%;height:auto;">
                    </v-flex>
                    <v-flex xs12 md6>
                      <v-card class="elevation-0 transparent">
                        <v-card-title primary-title class="layout justify-center">
                          <div class="headline text-xs-center">ciatr[シアター]</div>
                        </v-card-title>
                        <v-card-text>
                          ciatrは映画・ドラマ・アニメをもっと好きになるためのメディア。気になる情報や感想・評価・ネタバレや画像、動画を掲載しています。
                        </v-card-text>
                        <v-btn round outline color="blue" href="https://ciatr.jp" target="_brank" dark>Web Link<v-icon>launch</v-icon></v-btn>
                        <v-btn round outline color="blue" href="https://itunes.apple.com/jp/app/id1304288837?mt=8" target="_brank" dark>iOS App<v-icon>get_app</v-icon></v-btn>
                      </v-card>
                    </v-flex>
                  </v-layout>
                </v-container>
              </v-jumbotron>
            </v-flex>
          </v-flex>
        </div>

        <div class="about">
          <v-flex xs12 class="my-5 mx-3">
            <h1 class="headline text-xs-center">会社概要</h1>
            <v-jumbotron xs8 offset-xs2 height="auto">
              <v-flex class="mb-5 text-xs-left">
                <h1>MISSION</h1>
                <br />
                <span>物語との出会いを通して、人類に感動する機会を提供する</span>
              </v-flex>
              <v-flex class="mb-4 text-xs-left">
                <h1>会社概要</h1>
              </v-flex>
              <v-data-table
                :items="items"
                hide-actions
                hide-headers
              >
                <template slot="items" slot-scope="props">
                  <td class="text-xs-center">{{ props.item.calories }}</td>
                  <td class="text-xs-left">{{ props.item.name }}</td>
                </template>
              </v-data-table>
            </v-jumbotron>
          </v-flex>
        </div>

        <v-flex xs12 class="my-5">
          <h1 class="headline text-xs-center">求人情報</h1><br />
          <v-parallax :src="require('../assets/image.jpg')" height="300">
            <v-layout column align-center justify-center>
              <span class="subheading white--text">日本一の映画・ドラマ・アニメのエンタメサービスを目指すciatrで働きませんか？</span>
              <br /><br />
              <v-btn outline ripple large color="white" href="/recruit">求人情報はこちら
                <v-icon>work</v-icon>
              </v-btn>
            </v-layout>
          </v-parallax>
        </v-flex>

    </v-layout>
  </section>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      items: [
        {
          value: false,
          calories: '社名',
          name: '株式会社viviane'
        },
        {
          value: false,
          calories: '設立',
          name: '2012年3月14日'
        },
        {
          value: false,
          calories: '事業内容',
          name: 'Webサービスの企画・開発・運営'
        },
        {
          value: false,
          calories: '所在地',
          name: '〒150-0032 東京都渋谷区鶯谷町3-1 SUビル203'
        }
      ]
    }
  }
}
</script>

<style scoped>
.box {
  position: relative;
  width: 100%;
  height: 100%;
  padding-top: calc(500 / 1024 * 100%); /* calc(画像高さ ÷ 画像横幅 × 100%) */
  background: url('../assets/hero.jpg') center 20% / cover no-repeat;
}
.box::before{
  /* 透過した黒を重ねる */
  background-color: rgba(0,0,0,0.3);
  /* どの範囲に重ねるかを指定 */
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  content: ' ';
}
.hero {
  position: absolute;
  color: white;
  width: 80%;
  height: 50%;
  text-align: center;
  font-size: 6.5vw;
  top: 50%;
  left: 50%;
  -ms-transform: translate(-50%,-50%);
  -webkit-transform: translate(-50%,-50%);
  transform: translate(-50%,-50%);
  animation: fadeIn 2s ease 0s 1 normal;
  -webkit-animation: fadeIn 2s ease 0s 1 normal;
}
@keyframes fadeIn {
  0% {opacity: 0}
  100% {opacity: 1}
}
@-webkit-keyframes fadeIn {
  0% {opacity: 0}
  100% {opacity: 1}
}

</style>
