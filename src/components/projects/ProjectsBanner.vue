<template>
  <div class="projects-container">
    <ProjectCassette
      v-for="project in projects"
      :key="project.title"
      :project="project"
    />
  </div>
</template>


<script>
import ProjectCassette from "./ProjectCassette.vue";
export default {
  name: "ProjectsBanner",
  components: {
    ProjectCassette,
  },
  data() {
    return {
      projects: [
        {
          title: "Crypto Currency Tracker",
          description: "This is a crypto currency tracker using Nuxt.js and the CoinGecko API.",
          image: "/images/crypto-tracker.png",
          link: "https://www.google.com",
          language: "JavaScript",
          type: "Web",
        },
        {
          title: "Space Invaders Clone",
          description: "Space Invaders clone using HTML, CSS, and JavaScript.",
          image: "/images/space-invaders.png",
          link: "https://www.google.com",
          language: "HTML/CSS/JS",
          type: "Game",
        },
        // {
        //   title: "Weather App",
        //   description: "This is a description of project 3",
        //   image: "https://via.placeholder.com/150",
        //   link: "https://www.google.com",
        //   language: "JavaScript",
        //   type: "Web",
        // },
        {
          title: "2048 in Python",
          description: "2048 mathematical tile game made using PyGame.",
          image: "/images/2048.png",
          link: "https://www.google.com",
          language: "Python",
          type: "Game",
        },
      ],
      selected_project: null,
    };
  },
  methods: {},
};
</script>

<style scoped>
.projects-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-evenly;
  text-align: center;
  align-items: center;
  gap: 5px;
}
</style>