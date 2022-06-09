<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav>
  <router-view />
  <div>{{ nameHome }}</div>
  <button type="button" class="btn btn-primary">Primary</button>
</template>

<script>
export default {
  data() {
    return {
      nameHome: process.env.VUE_APP_NAME,
    };
  },
};
</script>

<style lang="scss">
@import "bootstrap";
</style>
