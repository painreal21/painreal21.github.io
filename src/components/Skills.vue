<template>
    <section class="skills-section">
      <h2 class="section-title" data-aos="fade-up">Technical Skills</h2>
      <div class="skills-bars">
        <div v-for="skill in skills" :key="skill.name" class="bar-container" data-aos="fade-up">
          <div class="bar-label">
            <strong>{{ skill.name }}</strong>
            <span>{{ skill.level }}%</span>
          </div>
          <div class="bar-bg">
            <div class="bar-fill" :style="{ width: skill.level + '%' }"></div>
          </div>
        </div>
      </div>
      <div class="skill-icons">
        <div v-for="icon in skillIcons" :key="icon.name" class="icon-card">
          <img :src="icon.src" :alt="icon.name" />
          <p>{{ icon.name }}</p>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    data() {
      return {
        skills: [
          { name: 'HTML5', level: 95 },
          { name: 'CSS3', level: 92 },
          { name: 'JavaScript', level: 90 },
          { name: 'Vue.js', level: 88 }
        ],
        skillIcons: [
          { name: 'HTML5', src: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg' },
          { name: 'CSS3', src: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg' },
          { name: 'JavaScript', src: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg' },
          { name: 'Vue.js', src: 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vuejs/vuejs-original.svg' }
        ]
      };
    }
  };
  </script>
  
  <style scoped>
  .skills-section {
    padding: 4rem 2rem;
    background-color: #111;
    color: #ffcfcf;
    text-align: center;
  }
  .section-title {
    font-size: 2rem;
    margin-bottom: 2rem;
    color: #ffa9a9;
  }
  .skills-bars {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 2rem;
  }
  .bar-container {
    width: 300px;
  }
  .bar-label {
    display: flex;
    justify-content: space-between;
    margin-bottom: 0.4rem;
  }
  .bar-bg {
    background: #333;
    height: 10px;
    border-radius: 5px;
  }
  .bar-fill {
    height: 10px;
    background: linear-gradient(to right, orange, yellow, cyan);
    border-radius: 5px;
  }
  .skill-icons {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    margin-top: 2rem;
    gap: 1.5rem;
  }
  .icon-card {
    background: #222;
    padding: 1rem;
    border-radius: 10px;
  }
  .icon-card img {
    width: 40px;
    height: 40px;
  }
  .icon-card p {
    margin-top: 0.5rem;
    color: #fff;
  }
  </style>
  