<template>
  <div>
    <h1 v-bind:style="colors">V-if</h1>
    <p v-if="isMe">I am {{ text }}</p>
    <p v-else>Who are you?</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      text: "text",
      isMe: false,
    };
  },
};
</script>