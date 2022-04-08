<template>
  <div id="vself">
    <div v-self="{}"></div>
  </div>
</template>


<script>
const app = Vue.createAPP({});
app.directive("self", {
  beforeMount(el, binding, vnode) {
    el.style.background = binding.value;
  },
});
</script>