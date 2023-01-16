<template>
  <div class="header">
    <h1 class="myName">Aankit Pokhrel</h1>
    <div class="bold-color">
      <button @click="Clicked" class="LinkedButton">Home</button>
      <button @click="Clicked" class="LinkedButton">Projects</button>
      <button href="https://github.com/AankitP" @click="OpenGitHub" class="LinkedButton">Github</button>
      <button @click="Clicked" class="LinkedButton">About Me</button>
      <button @click="Clicked" class="LinkedButton">Contact</button>
      <button href="./../assets/Aankit_Pokhrel_Resume.pdf" @click="OpenResume" class="LinkedButton">Resume</button>
        <!--This will be used for when I refactor the code and host the refactor -->
    </div>
  </div>
</template>

<script>

export default {
  methods: {
    Clicked() {
      console.log("Clicked");
    },
    OpenResume(){
      console.log("Clicked Open Resume");
      window.open("./../assets/Aankit_Pokhrel_Resume.pdf");
    },
    OpenGitHub(){
      console.log("Clicked Open GitHub");
      window.open("https://github.com/AankitP")
    }
  },
  name: "TopBar",
};

</script>

<style scoped>
.bold-color {
  color: aquamarine;
  font-weight: 800;
  display: flex;
  list-style: none;
  align-items: center;
  margin-right: .3rem;
}
.header {
  position: flex;
  background-color: #08355a;
  width: 100%;
  height: 4rem;
  /* border-bottom: 1px solid rgba(0, 0, 0, 0.301); */
  display: flex;
  justify-content: space-between;
}

h1 {
  color: aquamarine;
  font-size: 1.55rem;
  padding: 1rem;
  padding-left: 2rem;
  font-style: normal;
  font-weight: 900;
  line-height: 2rem;
}

.LinkedButton{
  background: none;
  border: none;
  color: aquamarine;
  font-weight: 800;
  padding: 1rem;
}

.LinkedButton:hover {
  background: #4174ff;
}

.header li {
  margin-right: 2rem;
  display: flex;
}

body{
  margin: 0 !important;
  padding: 0 !important;
}
</style>
