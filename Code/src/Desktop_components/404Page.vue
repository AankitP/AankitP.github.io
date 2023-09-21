<template>
  <div class="ItemHolder">
    <h1>
      Oops, this page is either being worked on, or I cannot show you yet.<br />
      Sorry for the inconvenience<br />
      To make this worth your time, here is a picture of a cute cat!
    </h1>
    <img src="./../assets/404Cat.jpg" class="OofImg" />
  </div>
</template>

<script>
// import { defineComponent } from '@vue/composition-api'
// import MainBox from "./Reusable/MainBox.vue";

export default {
  name: "OofPage",
  setup() {},
};
</script>

<style scoped>
.ItemHolder {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  width: auto;
  height: auto;
  margin: auto;
}
h1 {
  color: #ffffff;
}
.OofImg {
  max-height: 40rem;
  width: 20rem;
  border-radius: 10%;
  margin-top: 5%;
}
</style>
