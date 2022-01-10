<template>
  <v-app>
    <v-main>
      <Header />
      <nuxt />
    </v-main>
  </v-app>
</template>

<script lang="ts">
import Vue from "vue";
import Header from "@/components/Header.vue";

export default Vue.extend({
  components: {
    Header,
  },
});
</script>

<style lang="scss" scoped>
</style>