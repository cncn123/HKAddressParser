<template>
  <v-app>
    <v-toolbar app fixed clipped-left color="grey lighten-5 teal--text" >
      <v-toolbar-title>香港地址解析器 Hong Kong Address Parser</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items>
        <v-btn flat to="/">地圖模式</v-btn>
      </v-toolbar-items>
    </v-toolbar>
      <router-view/>
  </v-app>
</template>

<script>
const APP_VERSION = process.env.VUE_APP_REV_NAME;

export default {
  name: "App",
  data() {
    return {
      APP_VERSION
    };
  }
};
</script>
