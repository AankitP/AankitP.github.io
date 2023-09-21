<template>
  <div class="Content">
    <h1 class="ContactMe">Contact Me<br /></h1>
    <h1 class="PageDescriptor">You can contact me through Email:</h1>
    <div class="imgHolder">
      <a href="mailto:2001aankit@gmail.com"><img src="../assets/gmail.png" /></a>
    </div>
    <h1 class="Socials">Socials<br /></h1>
    <h1 class="PageDescriptor">Feel free to follow my socials:</h1>
    <div class="imgHolder">
      <a href="https://www.linkedin.com/in/aankit-pokhrel/" target="_blank"><img src="../assets/linkedin.png" /></a>
      <a href="https://www.instagram.com/aankit_pokhrel/" target="_blank"><img src="../assets/instagram.png" /></a>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContactPage",
  components: {},
};
</script>

<style scoped>
img {
  max-height: 12rem;
  width: auto;
}
.PageDescriptor {
  align-content: left;
  justify-content: left;
  text-align: left;
  color: #47ff94;
  font-size: 200%;
  margin-left: 3%;
}
.ContactMe {
  align-content: left;
  justify-content: left;
  text-align: left;
  color: #10c55c;
  font-size: 500%;
}
.Socials {
  align-content: left;
  justify-content: left;
  text-align: left;
  color: #10c55c;
  font-size: 500%;
}
.Content {
  color: #ffffff;
  justify-content: center;
  text-align: center;
  margin-top: 3%;
  margin-left: 4%;
  min-width: 50vw;
  width: auto;
}
.imgHolder {
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-content: center;
  margin: 5%;
}
</style>
