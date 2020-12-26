<template>
  <v-main>
    <section class="mv bg-light-gray">
      <v-container class="height-100vh">
        <h1 class="text-center text-h2 mb-4 mt-40vh font-weight-light">Kaito Kimura</h1>
        <v-row justify="center">
          <scroll-button
            link="#about"
            class="mx-auto"
          ></scroll-button>
        </v-row>
      </v-container>
    </section>
    <section id="about" class="py-10 about">
      <section-title>About me</section-title>
      <v-container>
        <v-row justify="center">
          <profile-card
            img-file="icon-profile.png"
            name="木村 海登"
          >専修大学 ネットワーク情報学部 ネットワーク情報学科 在学中。2022年度卒業予定。Webフロントエンド(Vue.js)を得意とし、Webサイトや小規模Webアプリケーションのフルスタック開発経験があります。</profile-card>
        </v-row>
      </v-container>
    </section>
    <section id="skills" class="py-10 skills bg-gray">
      <v-container>
        <section-title>Skills</section-title>
        <skills></skills>
      </v-container>
    </section>
    <section id="works" class="py-10 works bg-light-gray">
      <v-container>
        <section-title>Works</section-title>
        <works></works>
      </v-container>
    </section>
  </v-main>
</template>

<script>
import ScrollButton from '@/components/atoms/ScrollButton.vue';
import SectionTitle from '../atoms/SectionTitle.vue';
import ProfileCard from '@/components/molecules/ProfileCard.vue';
import Skills from '@/components/organisms/Skills.vue';
import Works from '@/components/organisms/Works.vue';
export default {
  components: {
    ScrollButton,
    SectionTitle,
    ProfileCard,
    Skills,
    Works,
  },

}
</script>


<style scoped>
  .height-100vh {
    height: 100vh;
  }
  .mt-40vh {
    margin-top: 30vh;
  }

  .bg-light-gray {
    background-color: #f3f3f3;
  }

  .bg-gray {
    background-color: #e2e2e2;
  }
</style>