<template>
  <v-app-bar>
    <v-app-bar-title>{{title}}</v-app-bar-title>
    <v-spacer></v-spacer>
    <v-tool-box>
      <v-btn v-for="menu in navMenues" :key="menu.title"></v-btn>
      <v-btn @click="goto(menu.link)">{{menu.title}}</v-btn>
      <v-btn>Works</v-btn>
    </v-tool-box>
  </v-app-bar>
</template>

<script>
export default {
  props: {
    title: {
      Type: String,
      Required: true
    },
    navMenus: {
      Type: Array,
      Requred: false,
    }
  },
  methods: {
    goto(link) {
      this.$vuetify.goTo(link);
    }
  }
}
</script>

<style>

</style>