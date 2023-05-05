<template>
  <div>
    <h1 v-bind:style="colors">V-bind</h1>

    <button @click="chageColor">Change Color</button>

    <br /><br />

    <button
      v-bind:class="{ green: boolean, blue: !boolean }"
      @click="boolean = !boolean"
    ></button>

    <h1 v-if="boolean">This is True</h1>
    <h1 v-else>This is False</h1>
    <br />

    <li v-for="animal in animals" :key="animal.id">{{ animal.name }}</li>

    <p>I like {{ animals[0].name }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      text: "text",
      colors: { color: "blue" },
      boolean: true,
      animals: [
        { id: 1, name: "Dog" },
        { id: 2, name: "Cat" },
        { id: 3, name: "Bird" },
        { id: 4, name: "Fish" },
      ],
    };
  },
  methods: {
    chageColor() {
      this.colors.color = "red";
    },
  },
};
</script>

<style scoped>
.green {
  background-color: green;
  width: 100px;
  height: 100px;
}

.blue {
  background-color: blue;
  width: 100px;
  height: 100px;
}
</style>