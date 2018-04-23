<template>
  <div class="product">
    <section>
      <v-layout
      column
      wrap
      class="my-5"
      align-center
      text-xs-center
      >
      <div class="my-5">
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
    </v-layout>
  </section>
</div>
</template>
