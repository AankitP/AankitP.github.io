<template>
  <div class="TextHolder">
    <h1 v-if="componentType === 'h1'">{{ data }}</h1>
    <h2 v-if="componentType === 'h2'">{{ data }}</h2>
    <h3 v-if="componentType === 'h3'">{{ data }}</h3>
    <h4 v-if="componentType === 'h4'">{{ data }}</h4>
    <p v-if="componentType === 'p'">{{ data }}</p>
  </div>
</template>

<script>
export default {
  name: "TextHolder",
  props: {
    data: String, // Define the 'data' prop and specify its type as String
    componentType: String, // Define the 'componentType' prop and specify its type as String
    style: String,
  },
};
</script>

<style scoped>
.TextHolder_Mobile {
  margin: 1rem;
  margin-right: 0.5rem;
  margin-left: 0.5rem;
  height: auto;
  display: flex;
  align-items: center;
  background-color: #08355a;
  border-radius: 1rem;
}
</style>
