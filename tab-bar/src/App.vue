<template>
  <div id="app">
    <router-view></router-view>
    <tab-bar></tab-bar>
  </div>
</template>

<script>
import TabBar from "./components/TabBar/TabBar";

export default {
  data() {
    return {};
  },
  components: {
    TabBar
  }
};
</script>

<style scope>
@import "./assets/css/base.css";
</style>
