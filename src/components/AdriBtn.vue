<template>
  <v-btn :class="classes" :disabled="disabled || loading">
    <v-progress-circular v-if="loading" :size="15" indeterminate></v-progress-circular>&nbsp;
    {{label}}
  </v-btn>
</template>

<script>
  export default {
    name: 'adri-btn',
    props: {
      label: String,
      loading: Boolean,
      disabled: Boolean,
      classes: String,
    },
  };
</script>

<style lang="scss" scoped>
  @import "../styles/ui-kit.scss";
</style>
