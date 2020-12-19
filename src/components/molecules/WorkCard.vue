<template>
  <v-col cols="11" lg="4">
    <v-card flat>
      <v-img
      contain
      height="280"
      max-width="400"
      :src="require('@/assets/img/' + imgFile)"></v-img>
      <h5 class="text-center">{{productName}}</h5>
      <p :class="subtitile">製作範囲</p>
      <p>{{range}}</p>
      <p :class="subtitile">使用言語</p>
      <p>{{languages}}</p>
      <p :class="subtitile">概要</p>
      <p><slot></slot></p>
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
    productName: {
      type: String,
      required: true,
    },
    range: {
      type: String,
      required: true,
    },
    languages: {
      type: String,
      required: true,
    },
  },
  data() {
    return {
      subtitile: ["font-weight-bold", "mb-0"],
    }
  }
}
</script>

<style>

</style>