<template>
  <div id="app">
    <router-link to="/home">首页</router-link>
    <router-link to="/about">关于</router-link>
    <!-- <router-link :to="userRouter">用户</router-link> -->
    <button @click="userClick">用户</button>
    <router-view />
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "cgy"
    };
  },
  methods: {
    userClick() {
      this.$router.push("/user/" + this.name);
    }
  }
};
</script>

<style>
</style>
