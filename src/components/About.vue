<template>
  <section class="about-section" id="about">
    <div class="about-container">
      <!-- Left: About Text -->
      <div class="about-text" data-aos="fade-right">
        <h2 class="about-title">About Me</h2>
        <p>
          I'm a passionate frontend developer with over 3 years of experience creating beautiful, functional websites that help businesses succeed online. My expertise lies in modern web technologies and creating user experiences that convert visitors into customers.
        </p>
        <p>
          I believe in clean code, responsive design, and the power of great user experience to drive business results. Every project I work on is crafted with attention to detail and optimized for performance.
        </p>

        <div class="features">
          <div class="feature-box">
            <i class="fas fa-code"></i>
            <div>
              <h4>Clean Code</h4>
              <p>Maintainable and scalable solutions</p>
            </div>
          </div>
          <div class="feature-box">
            <i class="fas fa-mobile-alt"></i>
            <div>
              <h4>Responsive</h4>
              <p>Perfect on all devices</p>
            </div>
          </div>
        </div>
      </div>

      <!-- Right: Developer Box -->
      <div class="about-graphic" data-aos="fade-left">
        <div class="dev-box">
          <span>Developer</span>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'About',
};
</script>

<style scoped>
.about-section {
  background: linear-gradient(to right, #111111, #1a1a1a);
  color: #fff;
  padding: 4rem 2rem;
}

.about-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  gap: 2rem;
  max-width: 1200px;
  margin: auto;
  align-items: center;
}

.about-text {
  flex: 1 1 500px;
}

.about-title {
  color: #ff6600;
  font-size: 2.5rem;
  margin-bottom: 1rem;
}

.about-text p {
  color: #ccc;
  margin-bottom: 1rem;
  line-height: 1.6;
}

.features {
  display: flex;
  gap: 1rem;
  margin-top: 2rem;
  flex-wrap: wrap;
}

.feature-box {
  background: #1c1c1c;
  padding: 1rem 1.5rem;
  border-radius: 10px;
  display: flex;
  align-items: center;
  gap: 1rem;
  flex: 1 1 220px;
}

.feature-box i {
  font-size: 1.5rem;
  color: #ff6600;
}

.feature-box:nth-child(2) i {
  color: #00e5ff;
}

.feature-box h4 {
  margin: 0;
  color: white;
}

.feature-box p {
  margin: 0;
  font-size: 0.875rem;
  color: #aaa;
}

.about-graphic {
  flex: 1 1 300px;
  display: flex;
  justify-content: center;
}

.dev-box {
  background: #ff5722;
  border-radius: 15px;
  padding: 6rem 3rem;
  font-size: 2rem;
  font-weight: bold;
  text-align: center;
  box-shadow: 0 0 50px rgba(255, 87, 34, 0.3);
  color: white;
}
</style>
