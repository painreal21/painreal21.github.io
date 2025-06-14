<template>
    <section class="projects-section">
      <h2 class="section-title" data-aos="fade-up">Featured Projects</h2>
      <div class="projects-grid">
        <div class="project-card" v-for="project in projects" :key="project.title" data-aos="fade-up">
          <div :class="['project-header', project.colorClass]">
            <h3>{{ project.title }}</h3>
          </div>
          <div class="project-body">
            <strong>{{ project.subtitle }}</strong>
            <p>{{ project.description }}</p>
            <div class="tech-stack">
              <span v-for="tech in project.tech" :key="tech">{{ tech }}</span>
            </div>
            <div class="buttons">
              <button class="demo">Live Demo</button>
              <button class="code">View Code</button>
            </div>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    data() {
      return {
        projects: [
          {
            title: 'E-commerce',
            subtitle: 'E-commerce Platform',
            description: 'Modern shopping experience with Vue.js',
            tech: ['Vue.js', 'CSS3', 'JavaScript'],
            colorClass: 'orange',
          },
          {
            title: 'Dashboard',
            subtitle: 'SaaS Dashboard',
            description: 'Clean admin interface with real-time data',
            tech: ['HTML5', 'Vue.js', 'CSS3'],
            colorClass: 'blue',
          },
          {
            title: 'Corporate',
            subtitle: 'Corporate Website',
            description: 'Professional business presence',
            tech: ['JavaScript', 'CSS3', 'HTML5'],
            colorClass: 'yellow',
          }
        ]
      };
    }
  };
  </script>
  
  <style scoped>
  .projects-section {
    padding: 4rem 2rem;
    background-color: #1c1c1c;
    color: #e6ffe6;
    text-align: center;
  }
  
  .section-title {
    font-size: 2rem;
    margin-bottom: 2rem;
    color: #b5ffcb;
  }
  
  .projects-grid {
    display: flex;
    gap: 1.5rem;
    flex-wrap: wrap;
    justify-content: center;
  }
  
  .project-card {
    background-color: #1a1a1a;
    width: 300px;
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 10px 25px rgba(0,0,0,0.6);
  }
  
  .project-header {
    color: white;
    font-size: 1.8rem;
    padding: 2rem 0;
    text-align: center;
  }
  
  .orange {
    background: linear-gradient(to bottom, #ff6a00, #ff6a00 60%, transparent 100%);
  }
  .blue {
    background: linear-gradient(to bottom, #00e6ff, #00e6ff 60%, transparent 100%);
  }
  .yellow {
    background: linear-gradient(to bottom, #ffe54c, #ffe54c 60%, transparent 100%);
  }
  
  .project-body {
    padding: 1rem;
    text-align: left;
    background: #111;
  }
  
  .tech-stack {
    margin: 1rem 0;
  }
  .tech-stack span {
    background: #ffbf00;
    padding: 5px 10px;
    margin: 3px;
    border-radius: 15px;
    font-size: 0.8rem;
    color: black;
    display: inline-block;
  }
  
  .buttons {
    display: flex;
    justify-content: space-between;
  }
  .demo, .code {
    padding: 8px 12px;
    border-radius: 8px;
    border: none;
    cursor: pointer;
  }
  .demo {
    background: #ff5722;
    color: white;
  }
  .code {
    background: #00e6ff;
    color: black;
  }
  </style>
  