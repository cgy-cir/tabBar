<template>
  <div>
    <p>用户</p>
    <p>{{id}}</p>
    <p>{{$route.name}}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  props: ["id"]
};
</script>
