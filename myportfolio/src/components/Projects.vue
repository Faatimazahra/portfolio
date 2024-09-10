<template>
    <section id="projects" class="py-5 bg-light">
      <div class="container">
        <h2>My Projects</h2>
        <div class="row">
          <div class="col-md-4" v-for="project in projects" :key="project.id">
            <div class="card mb-4">
              <img :src="project.image" class="card-img-top" alt="Project Image">
              <div class="card-body">
                <h5 class="card-title">{{ project.title }}</h5>
                <p class="card-text">{{ project.description }}</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: 'ProjectsSection',
    data() {
      return {
        projects: [
          { id: 1, title: 'Project 1', description: 'Description of project 1', image: 'https://via.placeholder.com/150' },
          { id: 2, title: 'Project 2', description: 'Description of project 2', image: 'https://via.placeholder.com/150' },
          // Add more projects here
        ]
      };
    }
  }
  </script>
  
  <style scoped>
  /* Add custom styles here */
  </style>
  