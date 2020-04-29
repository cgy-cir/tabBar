<template>
  <div id="app">
    <router-link to="/home">首页</router-link>
    <router-link to="/about">关于</router-link>
    <router-link :to="'/user/'+userId">用户</router-link>
    <router-view />
  </div>
</template>

<script>
export default {
  data() {
    return {
      userId: "lili"
    };
  }
};
</script>

<style>
</style>
