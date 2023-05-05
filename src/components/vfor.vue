<template>
  <div>
    <h1>V-for</h1>
    <ul>
      <li v-for="color in colors" :key="color.id">{{ color.name }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      colors: [
        { id: 1, name: "Red" },
        { id: 2, name: "reen" },
        { id: 3, name: "Blue" },
        { id: 4, name: "Orange" },
      ],
    };
  },
};
</script>