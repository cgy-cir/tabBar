<template>
  <div>
    <p>用户</p>
    <p>{{id}}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      a: 123
    };
  },
  computed: {
    id() {
      return this.$route.params.id;
    }
  }
};
</script>
