<template>
  <div>
    <h1>我是hello组件</h1>
  </div>
</template>

<script>
import { defineAsyncComponent } from '@vue/runtime-core';

export default {
    components:{
        AsyncPage: defineAsyncComponent(() => import("./components/AsyncComponent.vue")),
    },
  data() {
    return {
      msg: "我是hello组件的数据msg",
    };
  },
  methods: {},

</script>


<style lang="stylus" scoped></style>