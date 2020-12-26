<template>
  <v-row justify="center">
    <work-card
      img-file="works/img-onomatalk.png"
      productName="オノマトーク"
      range="デザイン,フロントエンド, バックエンド"
      languages="Vue.js, Vuetify, Django Rest Framework, Firebase"
      page-link="https://onomatalk.web.app/"
      github-link="https://github.com/kmr-rmjr/onomatalk_web"
    >専修大学3年次のカリキュラムであるプロジェクトでの成果物です。<br>
    痛みのオノマトペを翻訳することに特化したWebコミュニケータ ”オノマトーク” の開発において、デザイン、フロントエンド、バックエンドの全行程を担当致しました。<br>
    フロントエンドはVue CLIでSPAの実装を行い、Firebaseにデプロイしました。<br>
    バックエンドはDjango Rest FramewokでAPIの実装を行い、Vultrにデプロイしました。</work-card>
    <work-card
      img-file="works/img-watt-changer.png"
      productName="Watt Changer"
      range="デザイン,フロントエンド, バックエンド"
      languages="HTML, CSS, JavaScript"
      page-link="https://wattchanger.netlify.app/"
      github-link="https://github.com/kmr-rmjr/watt_changer"
    >電子レンジの温めを他のW数で行う際の時間を計算することができるアプリケーションです。プログラミング学習を始めて一番最初に制作したアプリケーションです。<br>
    JavaScroptでのDOM操作を一通り学習した際に、なにか作ってみようと思い作成しました。<br>
    JavaScriptフレームワークを使用せずに実装を行い、Netlifyにデプロイしました。


    </work-card>
    <work-card
      img-file="works/img-og_project_web.png"
      productName="2020年度 尾形プロジェクト ウェブサイト"
      range="デザイン,フロントエンド, バックエンド"
      languages="Vue.js, Vuetify"
      page-link="http://www.ne.senshu-u.ac.jp/~proj2020-7/"
      github-link="https://github.com/kmr-rmjr/og_project_web"
    >専修大学2020年度プロジェクトにて企画された、尾形プロジェクトのWebサイトです。<br>
    デザインからコーディングまでの全行程を担当いたしました。<br>
    Vue CLIとVuetifyを使用してフロントエンドを実装し、大学のサーバーにアップロードしました。<br>
    余談ですが、私は本プロジェクトで開発チームに所属し、プロジェクトの代表を務めさせていただきました。</work-card>

  </v-row>
</template>

<script>
import WorkCard from '../molecules/WorkCard.vue';

export default {
  components: {
    WorkCard,
  },
}
</script>

<style>

</style>