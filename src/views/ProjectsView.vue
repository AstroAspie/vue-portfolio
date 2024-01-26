<template>
  <div>
    <h1>Projects</h1>
    <p>Here's a list of all projects:</p>
    <ul>
      <li v-for="project in projects" :key="project.id">
        <router-link :to="{ name: 'ProjectDetails', params: { id: project.id } }">
          {{ project.name }}
        </router-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Projects',
  data () {
    return {
      projects: []
    }
  },
}
</script>