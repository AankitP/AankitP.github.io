<template>
  <div class="aboutMe">
    <div v-for="(text, key) in HPText.HomePageText" :key="key">
      <TextHolder :data="text.data" :componentType="text.type" />
    </div>
  </div>
  <div class="picOfMe">
    <img src="./../assets/IMG_5899.jpg" />
  </div>
</template>

<script>
import HPText from "./../assets/TextFiles/SiteText.json";
import TextHolder from "./../Universal_Components/TextHolder.vue";

export default {
  name: "HomePage",
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
  font-size: 200%;
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
  text-align: left;
}
h1 {
  text-color: aquamarine;
}
.shortDescription {
  margin: 4.5rem;
  margin-top: 0rem;
  width: auto;
  height: 20rem;
  text-align: left;
}

.picOfMe {
  max-height: 40rem;
  max-width: 25rem;
  margin-right: 10vw;
}

img {
  max-height: 100%;
  max-width: 100%;
  border-radius: 10%;
  display: block;
  aspect-ratio: "1.33" !important;
}
</style>
