<template>
  <div>
    <button @click="greet">挨拶</button>
    <p>{{ time }}</p>
  </div>
</template>

<script>
export default {
  name: "Abutton",
  data() {
    return {
      time: 0,
    };
  },
  methods: {
    greet() {
      var myDate = new Date();
      if (Number(myDate.getHours) <= 11 && Number(myDate.getHours) >= 0) {
        alert("おはようございます。");
      } else if (
        Number(myDate.getHours) <= 18 &&
        Number(myDate.getHours) >= 12
      ) {
        alert("こんにちは。");
      } else {
        alert("こんばんは");
      }
      this.time = Number(myDate.getHours);
    },
  },
};
</script>

