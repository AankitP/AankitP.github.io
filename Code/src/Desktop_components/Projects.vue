<template>
  <div class="Content">
    <h1 class="Title">Projects<br /></h1>
    <h1 class="PageDescriptor">
      These are some of the projects that I am currently Working on, or have
      worked on in the past
    </h1>
    <div class="Projects">
      <!-- Website -->
      <ProjHolder>
        <div class="allHolderProj">
          <div class="textHolderProj">
            <h3>
              Current Project:
              <a
                href="https://github.com/AankitP/AankitSiteVue"
                target="_blank"
              >
                Website Refactor
              </a>
            </h3>
            <h5>
              &emsp;Initially, the website was solely built using HTML and CSS,
              as my knowledge at that time was limited, preventing me from
              enhancing its appearance and functionality. However, after being
              introduced to REACT, I finally gained the capability to
              significantly improve both the aesthetics and performance of the
              website.
            </h5>
          </div>
          <img src="./../assets/VueSiteCode.png" class="ProjImg" />
        </div>
      </ProjHolder>

      <!-- MoDNS -->
      <ProjHolder>
        <div class="allHolderProj">
          <img src="./../assets/MUILogo.png" class="ProjImg" />
          <img src="./../assets/REACT_Logo.png" class="ProjImg" />
          <div class="textHolderProj">
            <h3>
              Current Project:
              <a href="https://github.com/MoDNS/MoDNS" target="_blank">MoDNS</a>
            </h3>
            <h5>
              &emsp;This project serves as my capstone, where I collaborated
              with a group of four other individuals to develop a modular DNS
              application. My role involves working closely with one of my team
              members to create the frontend portion of the project. For the
              frontend, we are utilizing REACT with MUI, while the backend and
              modules are being developed in RUST.
            </h5>
          </div>
        </div>
      </ProjHolder>

      <!-- Electric Edge -->
      <ProjHolder>
        <div class="allHolderProj">
          <div class="textHolderProj">
            <h3>
              Project:
              <a
                href="https://github.com/krishabbashyal/electric-edge"
                target="_blank"
                >Electric Edge</a
              >
            </h3>
            <h5>
              &emsp;I am currently assisting my cousin with a project centered
              around an Electric Charger Service. The concept involves creating
              a platform that streamlines the connection between electric
              vehicles and privately owned charging stations. The primary
              objective is to simplify the process for EV owners to locate and
              access charging stations while they are away from home.
              Additionally, the project aims to address the scarcity of charging
              options in areas with limited public charging infrastructure, thus
              enhancing the availability of charging stations.
            </h5>
          </div>
          <img src="./../assets/VUE_Logo.png" class="ProjImg" />
        </div>
      </ProjHolder>

      <!-- PythonAI -->
      <ProjHolder>
        <div class="allHolderProj">
          <img src="./../assets/PythonLogo.png" class="ProjImg" />
          <div class="textHolderProj">
            <h3>
              Current Task:
              <a href="https://github.com/AankitP/PythonAI" target="_blank"
                >PythonAI</a
              >
            </h3>
            <h5>
              &emsp;Currently, I am enrolled in a Udemy course on AI and Machine
              Learning. My objective is to leverage the knowledge and skills
              acquired from this course to develop AI applications for various
              purposes. As part of my learning process, I am diligently saving
              the code I write and taking detailed notes in a dedicated GitHub
              repository.
            </h5>
          </div>
        </div>
      </ProjHolder>
    </div>
  </div>
</template>

<script>
import ProjHolder from "./Reusable/ProjectHolder.vue";

export default {
  name: "ProjectsDone",
  components: {
    ProjHolder: ProjHolder,
  },
};
</script>

<style scoped>
.PageDescriptor {
  align-content: left;
  justify-content: left;
  text-align: left;
  color: #47ff94;
  font-size: 200%;
  margin-left: 3%;
}
.Title {
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
</style>
