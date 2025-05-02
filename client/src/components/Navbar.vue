<script setup>
import { ref, watch } from 'vue';
import { loadState, saveState } from '../utils/Store.js';
import Login from './Login.vue';

const theme = ref(loadState('theme') || 'light')

function toggleTheme() {
  theme.value = theme.value == 'light' ? 'dark' : 'light'
}

watch(theme, () => {
  document.documentElement.setAttribute('data-bs-theme', theme.value)
  saveState('theme', theme.value)
}, { immediate: true })

function scrollToTop() {
  window.scrollTo({
    top: 0,
    behavior: 'smooth',
  });
}

function scrollToElementById(elementId) {
  const element = document.getElementById(elementId);
  if (element) {
    const navbarHeight = document.querySelector('nav').offsetHeight; // Get the navbar height
    const elementPosition = element.getBoundingClientRect().top + window.scrollY; // Element's position relative to the document
    const offsetPosition = elementPosition - navbarHeight + 20; // Adjust with extra padding (10px)

    window.scrollTo({
      top: offsetPosition,
      behavior: 'smooth',
    });
  }
}

</script>

<template>
  <nav>
    <section class="container-fluid">
      <div class="row mx-5">
        <div class="col-12">
          <div class="bg-light rounded-pill mt-4 mb-5 p-2 d-flex justify-content-between shadow-light">
            <img class="navbar-brand" alt="logo" src="../assets/img/r-logo.png" height="65" />
            <div class="d-flex gap-5 align-items-center fs-5 fw-bold nav-button">
              <span @click="scrollToTop" class="hover-underline" role="button" title="Navigate To Home">Home</span>
              <span @click="scrollToElementById('skillsSection')" class="hover-underline" role="button"
                title="Navigate To Skills Section">Skills</span>
              <span @click="scrollToElementById('projectsSection')" class="hover-underline" role="button"
                title="Navigate To Projects Section">Projects</span>
              <span @click="scrollToElementById('aboutSection')" class="hover-underline" role="button"
                title="Navigate To About Section">About</span>
              <span @click="scrollToElementById('contactSection')" class="hover-underline" role="button"
                title="Navigate To Contact Section">Contact</span>
            </div>
            <div class="d-flex align-items-center fs-2 me-3 gap-2">
              <!-- TODO change this link to the actual LinkedIn Profile link when you manage to log into your LinkedIn account -->
              <a href="https://www.linkedin.com/in/roman-wernsing-514b0a323?trk=people-guest_people_search-card"
                target="_blank" title="Navigate to Roman Wernsings LinkedIn Profile Page">
                <span class="mdi mdi-linkedin text-dark"></span>
              </a>
              <a href="https://github.com/RMWernsing" target="_blank" title="Navigate to Roman Wernsings GitHub Page">
                <span class="mdi mdi-github text-dark"></span>
              </a>
            </div>
          </div>
        </div>
      </div>
    </section>
  </nav>
</template>

<style lang="scss" scoped>
a {
  text-decoration: none;
}

.nav-button {
  display: flex;
}

.nav-link {
  text-transform: uppercase;
}

.navbar-nav .router-link-exact-active {
  border-bottom: 5px solid var(--bs-success);
  border-bottom-left-radius: 0;
  border-bottom-right-radius: 0;
}

.hover-underline {
  border-bottom: 5px solid transparent;
  transition: border-bottom 125ms ease-in-out;
  transition: all 300ms ease-in-out;
  text-decoration: none;
  color: black;
}

.hover-underline:hover {
  transform: translateY(-.4rem);
  border-bottom: 5px solid rgb(0, 0, 0);
}

span {
  text-decoration: none;
}

.shadow-light {
  box-shadow: 0 30px 40px rgba(0, 0, 0, .1);
}

section {
  background: linear-gradient(to bottom,
      rgba(0, 0, 0, 0.469) 70%,
      rgba(255, 255, 255, 0) 100%),
    linear-gradient(180deg,
      rgba(0, 0, 0, 1) 0%,
      rgba(0, 0, 0, 0.54) 41%,
      rgba(247, 255, 247, 0) 77%);
  // backdrop-filter: blur(5px);
  // -webkit-backdrop-filter: blur(5px);
  width: 100%;
  z-index: 1000;
}

@media (max-width: 870px) {
  .nav-button {
    display: none;
  }
}
</style>
