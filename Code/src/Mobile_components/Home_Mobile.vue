<template>
  <div class="aboutMe">
    <!-- to iterate through the text -->
    <div v-for="(text, key) in HPText.HomePageText" :key="key">
      <TextHolder :data="text.data" :componentType="text.type" />
    </div>
    <img src="../assets/IMG_5899.jpg" alt="Your Image Alt Text" />
  </div>
</template>

<script>
// import Vue from "vue"; // Import Vue
import TextHolder from "./../Universal_Components/TextHolder.vue";
import HPText from "./../assets/TextFiles/SiteText.json";

export default {
  name: "HomePage_Mobile",
  components: {
    TextHolder,
  },
  data() {
    return {
      HPText: HPText,
    };
  },
};
</script>

<style scoped>
.helloWorld {
  align-content: left;
  justify-content: left;
  text-align: left;
  color: aquamarine;
  font-size: 150%;
}
.hook {
  align-content: left;
  justify-content: left;
  text-align: left;
  color: #47ff94;
  font-size: 400%;
}
.myName {
  align-content: left;
  justify-content: left;
  text-align: left;
  color: #10c55c;
  font-size: 500%;
}

.aboutMe {
  color: #ffffff;
  justify-content: center;
  text-align: center;
  margin: 3rem;
  min-width: 50vw;
  width: auto;
}
.shortDescription {
  margin: 4.5rem;
  margin-top: 0rem;
  width: 65vw;
  height: 20rem;
  text-align: left;
}

.picOfMe {
  max-height: 50vh;
  max-width: 65vw;
  margin-right: 10vw;
  align: center;
}

img {
  max-height: 100%;
  max-width: 100%;
  border-radius: 10%;
  display: block;
  aspect-ratio: "1.33" !important;
}
</style>
