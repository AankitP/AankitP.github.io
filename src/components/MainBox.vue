<template>
    <div class="holder">
        {{props.children}}
    </div>
</template>

<script>
export default {
  props: ['children'],
  name: "MainBox",
};
</script>

<style scoped>
.holder {
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
