<template>
    <nav class="navbar navbar-expand-lg navbar-light">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">FatimaZahra</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item">
              <a class="nav-link" href="#home-section">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#about-section">About</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#projects-section">Projects</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#skills-section">Skills</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#contact-section">Contact</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </template>
  
  <script>
  export default {
    name: 'NavbarComponent'
  }
  </script>
  
  <style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Amiri:wght@400;700&display=swap');
  
  .navbar {
    position: sticky;
    top: 0;
    z-index: 1000;
    border-radius: 40px; /* Rounded corners */
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2); /* Enhanced shadow */
    padding: 5px 20px; /* Add padding for better spacing */
    display: flex;
    justify-content: center; /* Center horizontally */
  }
  
  /* Navbar items */
  .navbar-nav {
    display: flex;
    align-items: center;
  }
  
  .navbar-brand {
    font-size: 2rem; /* Increase font size */
    font-family: 'Amiri', serif; /* Apply Arabic font */
    font-weight: bold; /* Make it bold */
  }
  
  /* Remove default shadow from navbar-light */
  .navbar-light {
    box-shadow: none;
  }
  </style>
  