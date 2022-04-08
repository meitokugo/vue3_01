<template>
  <div id="UPform">
    <p>USERNAME:</p>
    <br />
    <input v-model="name1" placeholder="input your name" />
    <br />
    <p>PASSWORD:</p>
    <input v-model="word" placeholder="input your password" />
    <br />
    <button @click="msg">LOGIN</button>
    <p>{{ name1 }}</p>
    <br />
    <p>{{ word }}</p>
    <br />
    <p>{{ username }}</p>
    <br />
    <p>{{ password }}</p>
  </div>
</template>

<script>
export default {
  name: "UPform",
  data() {
    return {
      username: "admin",
      password: "12345",
      name1: "",
      word: "",
    };
  },
  methods: {
    msg() {
      if (this.name1 == this.username && this.word == this.password) {
        alert("login succeed");
      } else {
        alert("login failed");
      }
    },
  },
};
</script>
