<template>
  <v-row justify="start">
    <language-card v-for="language in Languages" :key="language.name"
      :img-file="`languages/logo-${language.img}`"
      :language="language.name"
    ></language-card>
  </v-row>
</template>

<script>
import LanguageCard from '../molecules/LanguageCard.vue'
export default {
  components: {
    LanguageCard,
  },
  data() {
    return {
      Languages: [
        {name: "HTML5", img: 'html.svg'},
        {name: "CSS", img: 'css.svg'},
        {name: "JavaScript ES6", img: 'javascript.svg'},
        {name: "Vue.js", img: 'vuejs.svg'},
        {name: "Django", img: 'django.svg'},
        {name: "Django Rest Framework", img: 'django-rest-framework.svg'},
      ]
    }
  }
}
</script>

<style>

</style>
