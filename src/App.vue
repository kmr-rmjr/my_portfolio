<template>
  <v-app>
    <custom-header
      title="Kaito Kimura"
      :navMenue="HeaderNav"
    ></custom-header>
    <main-page></main-page>
    <custom-footer
      color="black"
      text="Kaito Kimura All Rights reserved."
    ></custom-footer>
  </v-app>
</template>

<script>
import CustomFooter from './components/molecules/CustomFooter.vue';
import CustomHeader from './components/molecules/CustomHeader.vue';
import MainPage from './components/pages/MainPage.vue';


export default {
  name: 'App',

  components: {
    MainPage,
    CustomFooter,
    CustomHeader,
  },

  data: () =>
    ({
      HeaderNav: [
        {title: "About me", link: "#about"},
        {title: "Skills", link: "#skills"},
        {title: "Works", link: "#works"},
        ]
  }),
};
</script>
