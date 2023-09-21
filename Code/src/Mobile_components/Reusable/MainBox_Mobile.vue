<template>
  <div class="holderBox">
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: "MainBox_Mobile",
};
</script>

<style scoped>
.holderBox {
  margin: 1rem;
  min-height: 80vh;
  height: auto;
  display: flex;
  align-items: center;
  background-color: #08355a;
  border-radius: 1rem;
}
</style>
