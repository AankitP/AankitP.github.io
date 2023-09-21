<template>
  <slot></slot>
</template>

<script>
export default {
  name: "ProjHolder",
  setup() {},
};
</script>

<style>
.allHolderProj {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  margin: 5%;
}

.textHolderProj {
  display: flex;
  flex-direction: column;
  text-align: left;
  width: 60%;
}

h5 {
  margin-left: 1rem;
}

.ProjImg {
  /* aspect-ratio: "original" !important; */
  max-height: 12rem;
  width: auto;
  border-radius: 1rem;
  margin-right: 5%;
  margin-left: 5%;
}
</style>
