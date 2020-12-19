<template>
  <v-col cols="6" lg="3">
    <v-card flat color="rgba(0,0,0,0)">
      <v-img
      width="120"
      height="120"
      :src="require('@/assets/img/' + imgFile)"
      :lazy-src="require('@/assets/img/' + imgFile)"
      class="ma-auto"
      ></v-img>
      <p class="text-center mt-2">{{language}}</p>
    </v-card>
  </v-col>
</template>

<script>
export default {
  props: {
    imgFile: {
      type: String,
      required: true,
    },
    language: {
      type: String,
      required: true,
    }
  }
}
</script>

<style>

</style>