<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About {{ name }}</router-link> |
    <router-link to="/form">Form</router-link>
  </div>
  <router-view />

  <button type="button" class="btn btn-primary">Primary</button>
</template>

<script>
export default {
  data () {
    return {
      name: process.env.VUE_APP_NAME
    }
  }
}
</script>

<style lang="scss">
// 引入 npm install 的 bootstrap
@import "bootstrap";
</style>
