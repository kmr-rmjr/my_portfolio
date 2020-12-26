<template>
  <v-col cols="6" sm="4" lg="2" class="mb-6">
    <v-card flat color="rgba(0,0,0,0)">
      <v-img
      contain
      width="100"
      height="100"
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