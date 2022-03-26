<template>
  <v-row justify="start">
    <language-card v-for="language in Languages" :key="language.name"
      :img-file="`languages/logo-${language.img}`"
      :language="language.name"
      :star="language.star"
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
        {name: "HTML5", img: 'html.svg', star: 4},
        {name: "CSS/Sass", img: 'css.svg', star: 4},
        {name: "JavaScript ES6", img: 'javascript.svg', star: 4},
        {name: "Vue.js", img: 'vuejs.svg', star: 3},
        {name: "Django", img: 'django.svg', star: 2},
        {name: "Django Rest Framework", img: 'django-rest-framework.png', star: 2},
      ]
    }
  }
}
</script>
