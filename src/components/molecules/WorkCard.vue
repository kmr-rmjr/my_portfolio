<template>
  <v-col cols="11" sm="11" lg="4">
    <v-card flat color="rgba(0, 0, 0, 0)" class="mb-16">
      <v-img
        class="mx-auto mb-4"
        contain
        max-width="500"
        :src="require(`@/assets/img/${imgFile}`)"
        :lazy-src="require(`@/assets/img/${imgFile}`)"
      ></v-img>
      <h5 class="text-center text-h6 text-lg-subtitle-1 font-weight-bold mb-2">{{productName}}</h5>
      <v-row justify="center" class="mb-9">
        <v-btn v-bind="btn" color="#435466" :href="pageLink">Link</v-btn>
        <v-btn v-bind="btn" :href="githubLink">GitHub</v-btn>
      </v-row>
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
    pageLink: {
      type: String,
      required: true,
    },
    githubLink: {
      type: String,
      required: true,
    },
  },
  data() {
    return {
      subtitile: ["font-weight-bold", "mb-0"],
      btn: {
        rounded: true,
        dark: true,
        target: '_blank',
        class: ['mx-2', "text-capitalize"],
      }
    }
  }
}
</script>