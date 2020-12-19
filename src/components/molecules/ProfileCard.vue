<template>
  <v-col cols="11" lg="6">
    <v-img
      :src="require('@/assets/img/' + imgFile)"
      width="30%"
      class="mx-auto"
    >
    </v-img>
    <h4 class="text-center my-2">{{name}}</h4>
    <p><slot></slot></p>
  </v-col>
</template>

<script>
export default {
  props: {
    imgFile: {
      Type: String,
      required: true,
    },
    name: {
      Type: String,
      required: true,
    },
  },
}
</script>

<style>

</style>