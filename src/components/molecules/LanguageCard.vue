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
      <p class="text-center mt-n3"><v-icon small v-for="n in 5" :key="n">{{stars(star, n)}}</v-icon></p>
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
    },
    star: {
      type: Number,
      required: true,
    }
  },
  methods: {
    stars(star, n) {
      if(n <= star) {
        return 'fas fa-star'
      }
      else {
        return 'far fa-star'
      }
    }
  }
}
</script>