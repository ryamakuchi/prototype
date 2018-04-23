<template>
  <div>
    <v-toolbar class="white" light fixed>
      <v-toolbar-title class="px-5 hidden-sm-and-down"><router-link to="/" exact><img src="../assets/logo.png" alt="logo"></router-link></v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="px-5 hidden-sm-and-down">
        <v-btn flat value="product" to="/product"><span>プロダクト</span></v-btn>
        <v-btn flat value="about" to="/about"><span>会社概要</span></v-btn>
        <v-btn flat value="recruit" to="/recruit"><span>求人情報</span></v-btn>
      </v-toolbar-items>
      <v-toolbar-items class="hidden-md-and-up">
        <v-btn flat value="viviane" to="/"><span>home</span></v-btn>
        <v-btn flat value="product" to="/product"><span>プロダクト</span></v-btn>
        <v-btn flat value="about" to="/about"><span>会社概要</span></v-btn>
        <v-btn flat value="recruit" to="/recruit"><span>求人情報</span></v-btn>
      </v-toolbar-items>
    </v-toolbar>
    <v-content class="mt-5">
      <nuxt/>
    </v-content>
    <v-footer height="auto" class="grey darken-3">
      <v-layout row wrap justify-center>
        <v-flex xs12 py-3 text-xs-center white--text>
          &copy; {{ new Date().getFullYear() }} <strong>viviane inc</strong>
        </v-flex>
      </v-layout>
    </v-footer>
  </div>
</template>

<style>
html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*, *:before, *:after {
  box-sizing: border-box;
  margin: 0;
}
</style>
