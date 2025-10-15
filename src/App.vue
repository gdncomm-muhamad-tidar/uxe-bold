<script setup>
import NavMenu from './components/NavMenu.vue'
</script>

<template>
  <div>
    <NavMenu />
    <section id="home" class="hero-section">
      <div class="hero-content">
        <h1>Welcome to UXE Bold</h1>
        <p>Your Next Generation Vue.js Application</p>
        <button class="cta-button">Get Started</button>
      </div>
    </section>
    <section id="features" class="content-section">
      <h2>Features</h2>
      <div class="features-grid">
        <div class="feature-card">
          <h3>Modern Design</h3>
          <p>Clean and responsive user interface built with Vue 3</p>
        </div>
        <div class="feature-card">
          <h3>Fast Performance</h3>
          <p>Optimized for speed and efficiency</p>
        </div>
        <div class="feature-card">
          <h3>Easy to Use</h3>
          <p>Intuitive and user-friendly experience</p>
        </div>
      </div>
    </section>
    <main>
    </main>
  </div>
</template>

<style scoped>
.hero-section {
  height: 80vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  background: linear-gradient(135deg, #42b883 0%, #347474 100%);
  color: white;
}

.hero-content {
  padding: 2rem;
}

.hero-content h1 {
  font-size: 3rem;
  margin-bottom: 1rem;
}

.hero-content p {
  font-size: 1.5rem;
  margin-bottom: 2rem;
}

.cta-button {
  padding: 1rem 2rem;
  font-size: 1.2rem;
  background-color: white;
  color: #42b883;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  transition: transform 0.3s ease;
}

.cta-button:hover {
  transform: translateY(-2px);
}

.content-section {
  padding: 4rem 2rem;
  max-width: 1200px;
  margin: 0 auto;
}

.content-section h2 {
  text-align: center;
  font-size: 2.5rem;
  margin-bottom: 3rem;
  color: #2c3e50;
}

.features-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
}

.feature-card {
  background: white;
  padding: 2rem;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  text-align: center;
}

.feature-card h3 {
  color: #42b883;
  margin-bottom: 1rem;
}
</style>
