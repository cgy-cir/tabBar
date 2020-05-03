<template>
  <div class="tab-bar">
    <tab-bar-item path="/home">
      <template v-slot:inactive>
        <img src="../../assets/img/home.svg" alt height="25px" />
      </template>
      <template v-slot:active>
        <img src="../../assets/img/home-active.svg" alt height="25px" />
      </template>
      <template v-slot:name>
        <div>首页</div>
      </template>
    </tab-bar-item>
    <tab-bar-item path="/category">
      <template v-slot:inactive>
        <img src="../../assets/img/category.svg" alt height="25px" />
      </template>
      <template v-slot:active>
        <img src="../../assets/img/category-active.svg" alt height="25px" />
      </template>
      <template v-slot:name>
        <div>分类</div>
      </template>
    </tab-bar-item>
    <tab-bar-item path="/cart">
      <template v-slot:inactive>
        <img src="../../assets/img/cart.svg" alt height="25px" />
      </template>
      <template v-slot:active>
        <img src="../../assets/img/cart-active.svg" alt height="25px" />
      </template>
      <template v-slot:name>
        <div>购物车</div>
      </template>
    </tab-bar-item>
    <tab-bar-item path="/profile">
      <template v-slot:inactive>
        <img src="../../assets/img/profile.svg" alt height="25px" />
      </template>
      <template v-slot:active>
        <img src="../../assets/img/profile-active.svg" alt height="25px" />
      </template>
      <template v-slot:name>
        <div>我的</div>
      </template>
    </tab-bar-item>
  </div>
</template>

<script>
import TabBarItem from "../TabBar/TabBarItem";
export default {
  components: {
    TabBarItem
  }
};
</script>
<style scoped>
.tab-bar {
  display: flex;
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  background-color: #f6f6f6;
  box-shadow: 0 -1px 1px rgba(100, 100, 100, 0.2);
}
</style>