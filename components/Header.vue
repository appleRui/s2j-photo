<template>
  <v-toolbar dense fixed flat="true" class="header">
    <div class="header__content">
      <v-avatar size="20" tile> 📸 </v-avatar>
      <span class="header__content_ttl">Tokyo Denki University s2j-photo</span>
    </div>
  </v-toolbar>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({});
</script>

<style lang="scss" scoped>
.header {
  width: 100%;
  position: sticky;
  top: 0;
  left: 0;
  &__content {
    &_ttl {
      font-size: 14px;
      margin-left: 0.25rem;
    }
  }
}
</style>