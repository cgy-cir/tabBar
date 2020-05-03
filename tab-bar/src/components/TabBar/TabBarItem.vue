<template>
  <div class="tab-bar-item" @click="itemClick">
    <div v-if="!isActive">
      <slot name="inactive"></slot>
    </div>
    <div v-else>
      <slot name="active"></slot>
    </div>
    <div :class="{active:isActive}">
      <slot name="name"></slot>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    path: {
      type: String
    }
  },
  data() {
    return {};
  },
  computed: {
    isActive() {
      return this.$route.path.indexOf(this.path) !== -1;
    }
  },
  methods: {
    itemClick() {
      if (this.$route.path !== this.path) {
        this.$router.replace(this.path);
      }
    }
  }
};
</script>

<style scope>
.tab-bar-item {
  flex: 1;
  text-align: center;
  height: 49px;
  font-size: 14px;
  margin-top: 3px;
}

.tab-bar-item img {
  vertical-align: top;
}
.active {
  color: #1296db;
}
</style>