<template>
  <v-toolbar dense elevation="0" class="header">
    <div class="header__content">
      <v-avatar size="20" tile>
        <img src="@/assets/logo.png" alt="Logo" />
      </v-avatar>
      <span class="header__content_ttl">TDU 二部写真部</span>
    </div>
  </v-toolbar>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({});
</script>

<style lang="scss" scoped>
.header {
  &__content {
    &_ttl {
      margin-left: 0.25rem;
    }
  }
}
</style>