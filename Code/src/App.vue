<template>
  <header>
    <TopBar v-if="DeviceType == 'Desktop'" class="topBar" @clicked="getPage" />
  </header>
  <div class="allHolderDesktop" v-if="DeviceType == 'Desktop'">
    <MainBox>
      <HomePage v-if="accessThis == 'Home'" />
      <ProjectsDone v-else-if="accessThis == 'Projects'" />
      <ContactPage v-else-if="accessThis == 'Contact'" />
      <AboutMe v-else-if="accessThis == 'AboutMe'" />
      <OofPage v-else />
    </MainBox>
  </div>
  <div class="allHolderMobile" v-if="DeviceType == 'Mobile'">
    <MainBox_Mobile>
      <Home_Mobile v-if="accessThis == 'Home'" />
      <ProjectsDone v-else-if="accessThis == 'Projects'" />
      <ContactPage v-else-if="accessThis == 'Contact'" />
      <AboutMe v-else-if="accessThis == 'AboutMe'" />
      <OofPage v-else />
    </MainBox_Mobile>
  </div>
</template>

<script>
// Import desktop components
import TopBar from "./Desktop_components/TopBar.vue";
import MainBox from "./Desktop_components/Reusable/MainBox.vue";
import HomePage from "./Desktop_components/Home.vue";
import ProjectsDone from "./Desktop_components/Projects.vue";
import ContactPage from "./Desktop_components/ContactAndSocials.vue";
import OofPage from "./Desktop_components/404Page.vue";
import AboutMe from "./Desktop_components/AboutMe.vue";

// Import mobile components
import Home_Mobile from "./Mobile_components/Home_Mobile.vue";
import MainBox_Mobile from "./Mobile_components/Reusable/MainBox_Mobile.vue";

const DeviceType = () =>
  /Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(
    navigator.userAgent
  )
    ? "Mobile"
    : "Desktop";
console.log(DeviceType()); // "Mobile" or "Desktop"

export default {
  data: function () {
    return {
      accessThis: "Home",
      DeviceType: DeviceType(),
    };
  },
  name: "App",
  components: {
    TopBar,
    MainBox,
    HomePage,
    ProjectsDone,
    ContactPage,
    OofPage,
    AboutMe,
    Home_Mobile,
    MainBox_Mobile,
  },
  methods: {
    getPage(value) {
      this.accessThis = value;
    },
    getDeviceType() {
      this.DeviceType =
        /Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(
          navigator.userAgent
        )
          ? "Mobile"
          : "Desktop";
      console.log(this.DeviceType); // "Mobile" or "Desktop"
    },
  },
};
</script>

<style>
html {
  background-color: #175588;
  width: auto;
  height: auto;
}
body {
  background-color: #175588;
}
.allHolderDesktop {
  padding: 0 !important;
  margin: 0 !important;
  /* min-width: 100rem; */
  height: auto;
  background-color: #175588;
}
</style>
