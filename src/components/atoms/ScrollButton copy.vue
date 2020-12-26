<template>
  <v-col cols="5" lg="2">
    <v-img :src="require('@/assets/img/img-scroll-parts.png')"></v-img>
    <v-img
      :src="require('@/assets/img/icon-scroll-button.svg')"
      width="60%"
      class="mx-auto mt-2 pointer"
      @click="goto(link)"
    ></v-img>
  </v-col>
</template>

<script>
export default {
  props: {
    link: {
      type: String,
      required: true,
    }
  },
  methods: {
    goto(link) {
      this.$vuetify.goTo(link);
    }
  }
}
</script>

<style scoped>
  .pointer {
    cursor: pointer;
  }

  .pointer:hover {
    opacity: .7;
  }
</style>