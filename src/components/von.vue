<template>
  <div>
    <h1>V-on</h1>

    <input :value="text" v-on:input="convertToUpperCase" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      text: "text",
    };
  },
  methods: {
    convertToUpperCase(event) {
      this.text = event.target.value.toUpperCase();
    },
  },
};
</script>