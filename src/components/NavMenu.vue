<script setup>
const scrollToSection = (sectionId) => {
  const element = document.querySelector(sectionId);
  if (element) {
    element.scrollIntoView({ behavior: 'smooth', block: 'start' });
  }
};
</script>

<template>
  <nav class="nav-menu">
    <div class="nav-brand">
      <img alt="Vue logo" class="logo" src="../assets/logo.svg" width="40" height="40" />
      <span class="brand-name">UXE Bold</span>
    </div>
    <div class="nav-links">
      <a @click.prevent="scrollToSection('#home')" href="#home" class="nav-link">Home</a>
      <a @click.prevent="scrollToSection('#features')" href="#features" class="nav-link">Features</a>
      <a @click.prevent="scrollToSection('#about')" href="#about" class="nav-link">About</a>
      <a @click.prevent="scrollToSection('#contact')" href="#contact" class="nav-link">Contact</a>
    </div>
  </nav>
</template>

<style scoped>
.nav-menu {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  background-color: #ffffff;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1000;
}

.nav-brand {
  display: flex;
  align-items: center;
  gap: 1rem;
}

.brand-name {
  font-size: 1.5rem;
  font-weight: bold;
  color: #42b883;
}

.nav-links {
  display: flex;
  gap: 2rem;
}

.nav-link {
  text-decoration: none;
  color: #2c3e50;
  font-weight: 500;
  transition: color 0.3s ease;
}

.nav-link:hover {
  color: #42b883;
}

@media (max-width: 768px) {
  .nav-menu {
    flex-direction: column;
    gap: 1rem;
    padding: 1rem;
  }

  .nav-links {
    flex-direction: column;
    align-items: center;
    gap: 1rem;
  }
}
</style>