<template>
  <div>
    <h1>Test</h1>

    <p v-for="maun in manufacturer" :key="maun.id">{{ maun.title }}</p>
  </div>
</template>

<script>
import axios from "axios";

export default {
  data() {
    return {
      text: "text",
      manufacturer: [{ id: 1, title: "test1" }],
    };
  },
  created() {
    this.get();
  },
  methods: {
    get() {
      axios
        .get("https://localhost:7203/api/manufacturer")
        .then((respone) => (this.manufacturer = respone.data));
    },
  },
};
</script>