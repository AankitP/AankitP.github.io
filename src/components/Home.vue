<template>
  <div class="holder">
    <div class="aboutMe">
      <p class="helloWorld">
        Hello World, My Name is 
      </p>
      <h1 class="myName">
        Aankit Pokhrel.<br/>
      </h1>
      <h1 class="hook">
        And I Build Things for Fun.
      </h1>
      <div class="shortDescription">
        <p>
          I am A senior Cyber Engineering Major at Louisiana Tech university<br/>
          currently a working on my capstone<br/>
          and am Projected to graduate in May 2023
        </p>
      </div>
    </div>
    <div class="PicOfMe">
      <img src="./../assets/IMG_5899.jpg"/>
    </div>
  </div>
</template>

<script>
export default {
  name: "AboutMe",
};
</script>


<style scoped>
.helloWorld{
  align-content: left;
  justify-content: left;
  text-align: left;
  color:aquamarine;
  font-size: 200%;
}
.hook{
  align-content: left;
  justify-content: left;
  text-align: left;
  color: #47ff94;
  font-size: 400%;
}
.myName{
  align-content: left;
  justify-content: left;
  text-align: left;
  color: #10c55c;
  font-size: 500%;
}
.holder{
  margin: 4rem;
  margin-right: 4rem;
  margin-left: 2rem;
  min-height: 80vh;
  height: auto;
  min-width: 300rem;
  width: auto;
  display: flex;
  align-items: center;
  background-color: #08355a;
  border-radius: 1rem;
}
.aboutMe {
  color: #ffffff;
  justify-content: center;
  text-align: center;
  margin: 3rem;
  min-width: 50vw;
  width: auto;
}
.shortDescription{
  margin: 4.5rem;
  margin-top: 0rem;
  width: 65vw;
  height: 20rem;
  text-align: left;
}
img{
  max-height: 40rem;
  max-width: 40rem;
  margin-right: 10vw;
  border-radius: 2rem;
  aspect-ratio: "1.33";
}
</style>