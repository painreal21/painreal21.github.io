<template>
  <div class="home">
    <section class="hero" data-aos="fade-up">
      <h1>
        <span class="highlight">Frontend</span> Developer
      </h1>
      <p>
        I create stunning, responsive websites that drive business growth.
        Specializing in modern web technologies to deliver exceptional user
        experiences that convert.
      </p>
      <div class="buttons">
        <a href="#projects" class="btn-orange">View My Work</a>
        <a href="#contact" class="btn-blue">Get In Touch</a>
      </div>

      <div class="stats">
        <div class="stat" data-aos="fade-up" data-aos-delay="100">
          <h2 class="orange">50+</h2>
          <p>Projects Completed</p>
        </div>
        <div class="stat" data-aos="fade-up" data-aos-delay="200">
          <h2 class="blue">3+</h2>
          <p>Years Experience</p>
        </div>
        <div class="stat" data-aos="fade-up" data-aos-delay="300">
          <h2 class="yellow">100%</h2>
          <p>Client Satisfaction</p>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isMenuOpen: false,
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    },
  },
};
</script>

<style scoped>
@import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css');

body {
  margin: 0;
  font-family: 'Segoe UI', sans-serif;
  background: radial-gradient(circle at left, #1f0d0d, #001f1f);
  color: #fff;
}

.hero {
  text-align: center;
  padding: 4rem 2rem;
}

.hero h1 {
  font-size: 3rem;
  margin-bottom: 1rem;
  background: linear-gradient(to right, #ffb347, #00ffff);
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.hero p {
  font-size: 1rem;
  max-width: 600px;
  margin: 0 auto 2rem;
  color: #ccc;
}

.buttons {
  display: flex;
  justify-content: center;
  gap: 1rem;
  margin-bottom: 3rem;
}

a.btn-orange {
  background-color: #ff5722;
  color: white;
  padding: 0.75rem 1.5rem;
  border: none;
  border-radius: 8px;
  font-weight: bold;
  text-decoration: none;
  box-shadow: 0 4px 12px #ff5722;
  transition: 0.3s;
}

a.btn-orange:hover {
  background-color: #e04e1c;
  box-shadow: 0 6px 14px #e04e1c;
}

a.btn-blue {
  background-color: transparent;
  color: #00e5ff;
  border: 2px solid #00e5ff;
  padding: 0.75rem 1.5rem;
  border-radius: 8px;
  font-weight: bold;
  text-decoration: none;
  box-shadow: 0 4px 12px #00e5ff;
  transition: 0.3s;
}

a.btn-blue:hover {
  background-color: #00e5ff;
  color: #000;
  box-shadow: 0 6px 14px #00e5ff;
}

.stats {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 2rem;
}

.stat {
  background: #1c1c1c;
  padding: 2rem;
  border-radius: 10px;
  text-align: center;
  width: 180px;
}

.stat h2 {
  font-size: 2rem;
  margin-bottom: 0.5rem;
}

.stat h2.orange {
  color: #ff6600;
}

.stat h2.blue {
  color: #00e5ff;
}

.stat h2.yellow {
  color: #ffb347;
}

.stat p {
  color: #aaa;
}

/* Responsive */
@media (max-width: 768px) {
  .buttons {
    flex-direction: column;
  }
}
</style>
