<template>
  <div>
    <div id="change" :class="[right ? active : error]">here was red</div>
  </div>
</template>

<script>
export default {
  name: "change",
  data() {
    return {
      right: true,
      active: "active",
      error: "danger",
    };
  },
};
</script>

<style scoped>
.active {
  background-color: blue;
  height: 300px;
  width: 300px;
}

.danger {
  background: red;
  height: 300px;
  width: 300px;
}
</style>


