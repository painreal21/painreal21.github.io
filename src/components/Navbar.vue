<template>
  <header class="navbar">
    <div class="logo">Ben's<span style="color: orange">Portfolio</span></div>

    <div class="hamburger" @click="toggleMenu">
      <span></span>
      <span></span>
      <span></span>
    </div>

    <nav :class="['navigation', { 'open': isMenuOpen }]">
      <a href="#home" @click="closeMenu">Home</a>
      <a href="#about" @click="closeMenu">About</a>
      <a href="#projects" @click="closeMenu">Projects</a>
      <a href="#skills" @click="closeMenu">Skills</a>
      <a href="#contact" @click="closeMenu">Contact</a>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Navbar',
  data() {
    return {
      isMenuOpen: false,
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    },
    closeMenu() {
      this.isMenuOpen = false;
    },
  },
}
</script>

<style scoped>
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  background-color: #111;
  position: fixed;
  top: 0;
  width: 80%;
  z-index: 1000;
  box-shadow: 0 2px 5px rgba(0,0,0,0.2);
}

.logo {
  font-weight: bold;
  font-size: 24px;
  color: white;
}

.navigation {
  display: flex;
  gap: 1rem;
}

.navigation a {
  color: white;
  text-decoration: none;
  transition: color 0.3s;
}

.navigation a:hover {
  color: orange;
}

/* Hamburger Icon */
.hamburger {
  display: none;
  flex-direction: column;
  cursor: pointer;
  gap: 5px;
}

.hamburger span {
  width: 25px;
  height: 3px;
  background-color: white;
  border-radius: 2px;
}

/* Responsive Styles */
@media (max-width: 768px) {
  .hamburger {
    display: flex;
  }

  .navigation {
    position: absolute;
    top: 60px;
    right: 0;
    background-color: #111;
    flex-direction: column;
    width: 100%;
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.3s ease-out;
  }

  .navigation.open {
    max-height: 300px; /* enough to show all links */
  }

  .navigation a {
    padding: 1rem;
    text-align: center;
    border-top: 1px solid #222;
  }
}
</style>
