<template>
  <div>
    <h1>Prop</h1>
    <p>{{ text }}</p>
    <input v-model="text" />
    <button @click="goToHome()">Go</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      text: "",
    };
  },
  methods: {
    goToHome() {
      this.$router.push({ path: "/", query: { msg: this.text } });
    },
  },
};
</script>