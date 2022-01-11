<template>
  <NotionRenderer :blockMap="blockMap" fullPage />
</template>

<script lang="ts">
import Vue from "vue";
import { NotionRenderer, getPageBlocks } from "vue-notion";

type blockMap = {
  blockMap: Array<Object>;
};

export default Vue.extend({
  components: {
    NotionRenderer,
  },
  data() {
    return {
      blockMap: [],
    };
  },
  async created() {
    this.blockMap = await getPageBlocks(this.$config.PageId);
  },
});
</script>

<style>
@import "vue-notion/src/styles.css";
@import "@/assets/style/overrides.css";
</style>
