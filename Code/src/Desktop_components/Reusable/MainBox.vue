<template>
  <div class="holderBox">
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: "MainBox",
};
</script>

<style scoped>
.holderBox {
  margin: 4rem;
  margin-right: 4rem;
  margin-left: 4rem;
  min-height: 80vh;
  height: auto;
  display: flex;
  align-items: center;
  background-color: #08355a;
  border-radius: 1rem;
}
</style>
