<template>
  <v-footer>
    <p>{{text}}</p>
  </v-footer>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      required: true,
    }
  }
}
</script>

<style>

</style>