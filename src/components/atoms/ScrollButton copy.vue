<template>
  <v-col cols="8" lg="2">
    <v-card v-bind="circle"></v-card>
    <v-card v-bind="circle"></v-card>
    <p class="text-center my-2">Pleace Scroll Down</p>
    <v-card v-bind="circle"></v-card>
    <v-card v-bind="circle"></v-card>
    <v-img
      :src="require('@/assets/img/icon-scroll-button.svg')"
      width="40%"
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
  data() {
    return {
      circle: {
        width: 15,
        height: 15,
        color: '#333',
        class: ['mx-auto', 'rounded-circle', 'my-3']
      }
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