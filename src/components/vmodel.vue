<template>
  <div>
    <h1>V-model</h1>
    <p>{{ text }}</p>
    <input v-model="text" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      text: "text",
    };
  },
};
</script>