<template>
  <div v-if="isLoading" class="min-h-screen bg-gray-900 flex items-center justify-center">
  <div class="text-center">
    <div ref="spinnerContainer" class="mb-4 flex justify-center"></div>
    <p class="text-blue-400 text-2xl font-bold mt-4">{{ countdownText }}</p>
  </div>
  </div>
  <div v-else class="min-h-screen bg-gray-900 relative text-white">
    <Navbar />
    <main class="container mx-auto px-4 py-8">
      <Hero />
      <About />
      <Skills />
      <Experience />
      <Education />
      <Projects />
      <Contact />
    </main>
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Hero from './components/Hero.vue'
import About from './components/About.vue'
import Skills from './components/Skills.vue'
import Experience from './components/Experience.vue'
import Education from './components/Education.vue'
import Projects from './components/Projects.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'
import { quantum } from 'ldrs'

export default {
  name: 'App',
  components: {
    Navbar,
    Hero,
    About,
    Skills,
    Experience,
    Education,
    Projects,
    Contact,
    Footer
  },
  data() {
    return {
      isLoading: true,
      countdown: 3,
      countdownText: ''
    }
  },
    mounted() {
    // Register the dot spinner
    quantum.register()
    
    // Create and add the spinner element
    const spinner = document.createElement('l-quantum')
    spinner.setAttribute('size', '55')
    spinner.setAttribute('speed', '1.75')
    spinner.setAttribute('color', '#38bdf8') // Use your blue color
    
    this.$refs.spinnerContainer.appendChild(spinner)
    
    // Start countdown
    this.startCountdown()
  },
  
  methods: {
    startCountdown() {
      // Initial countdown text
      this.countdownText = `Loading in ${this.countdown}...`
      
      // Set up countdown interval
      const countdownInterval = setInterval(() => {
        this.countdown -= 1
        
        if (this.countdown <= 0) {
          // Clear the interval when countdown reaches 0
          clearInterval(countdownInterval)
          this.countdownText = 'Welcome!'
          
          // Show the main content after a brief pause
          setTimeout(() => {
            this.isLoading = false
          }, 500)
        } else {
          // Update countdown text
          this.countdownText = `Loading in ${this.countdown}...`
        }
      }, 1000)
    }
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');

body {
  font-family: 'Poppins', sans-serif;
  margin: 0;
  padding: 0;
}

.section-title {
  @apply text-3xl font-bold mb-8 text-center;
  background: linear-gradient(to right, #38bdf8, #818cf8);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
</style>