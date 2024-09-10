<template>
    <section id="skills" class="py-5">
      <div class="container">
        <h2>Skills</h2>
        <div class="row">
          <div class="col-md-3" v-for="skill in skills" :key="skill.id">
            <div class="skill-item">
              <h5>{{ skill.name }}</h5>
              <p>{{ skill.level }}</p>
            </div>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: 'SkillsSection',
    data() {
      return {
        skills: [
          { id: 1, name: 'HTML & CSS', level: 'Advanced' },
          { id: 2, name: 'Vue.js', level: 'Intermediate' },
          // Add more skills here
        ]
      };
    }
  }
  </script>
  
  <style scoped>
  /* Add custom styles here */
  </style>
  