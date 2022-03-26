<template>
  <v-footer dark height="70px">
    <p class="ma-auto">{{text}}</p>
  </v-footer>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      required: true,
    },
  }
}
</script>