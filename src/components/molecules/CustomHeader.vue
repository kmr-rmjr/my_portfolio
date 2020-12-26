<template>
  <v-app-bar dark app>
    <template v-if="$vuetify.breakpoint.xs"></template>
    <template v-else>
      <v-toolbar-title>{{title}}</v-toolbar-title>
      <v-spacer></v-spacer>
    </template>
    <v-toolbar-items class="mx-auto">
      <v-btn text v-for="menu in navMenue" :key="menu.title" @click="goto(menu.link)">{{menu.title}}</v-btn>
    </v-toolbar-items>
  </v-app-bar>
</template>

<script>
export default {
  props: {
    title: {
      Type: String,
      Required: true
    },
    navMenue: {
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