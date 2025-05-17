<template>
  <nav class="bg-opacity-20 bg-black backdrop-filter backdrop-blur-lg fixed w-full z-10">
    <div class="container mx-auto px-4">
      <div class="flex justify-between items-center py-4">
        <div class="text-xl font-bold">
          <span class="bg-clip-text text-transparent bg-gradient-to-r from-blue-400 to-purple-500">
            Alvin Kimutai
          </span>
        </div>
        <div class="hidden md:flex space-x-8">
          <a href="#about" class="hover:text-blue-300 transition-colors">About</a>
          <a href="#skills" class="hover:text-blue-300 transition-colors">Skills</a>
          <a href="#experience" class="hover:text-blue-300 transition-colors">Experience</a>
          <a href="#education" class="hover:text-blue-300 transition-colors">Education</a>
          <a href="#projects" class="hover:text-blue-300 transition-colors">Projects</a>
          <a href="#contact" class="hover:text-blue-300 transition-colors">Contact</a>
        </div>
        <div class="md:hidden">
          <button @click="toggleMenu" class="focus:outline-none">
            <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
              <path v-if="!isMenuOpen" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
              <path v-else stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
            </svg>
          </button>
        </div>
      </div>
      
      <!-- Mobile menu -->
      <div v-if="isMenuOpen" class="md:hidden">
        <div class="flex flex-col space-y-4 pb-4">
          <a href="#about" class="hover:text-blue-300 transition-colors" @click="closeMenu">About</a>
          <a href="#skills" class="hover:text-blue-300 transition-colors" @click="closeMenu">Skills</a>
          <a href="#experience" class="hover:text-blue-300 transition-colors" @click="closeMenu">Experience</a>
          <a href="#education" class="hover:text-blue-300 transition-colors" @click="closeMenu">Education</a>
          <a href="#projects" class="hover:text-blue-300 transition-colors" @click="closeMenu">Projects</a>
          <a href="#contact" class="hover:text-blue-300 transition-colors" @click="closeMenu">Contact</a>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'SiteNavbar',
  data() {
    return {
      isMenuOpen: false
    }
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen
    },
    closeMenu() {
      this.isMenuOpen = false
    }
  }
}
</script>