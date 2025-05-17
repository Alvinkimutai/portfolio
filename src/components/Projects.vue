<template>
  <section id="projects" class="py-20">
    <h2 class="section-title">Projects</h2>
    
    <div class="max-w-6xl mx-auto">
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
        <!-- Project 1 -->
        <div class="bg-white bg-opacity-5 rounded-xl overflow-hidden hover:transform hover:scale-105 transition-all duration-300">
          <div class="h-48 overflow-hidden">
            <img src="https://via.placeholder.com/600x400" alt="Project 1" class="w-full h-full object-cover" />
          </div>
          <div class="p-6">
            <h3 class="text-xl font-bold mb-2 text-blue-300">Smart Building Management System</h3>
            <p class="text-gray-300 mb-4">
              A web application that combines IoT sensors with building information modeling to optimize energy usage and maintenance.
            </p>
            <div class="flex flex-wrap gap-2 mb-4">
              <span class="text-xs bg-blue-900 bg-opacity-50 px-2 py-1 rounded-full">Vue.js</span>
              <span class="text-xs bg-blue-900 bg-opacity-50 px-2 py-1 rounded-full">Node.js</span>
              <span class="text-xs bg-blue-900 bg-opacity-50 px-2 py-1 rounded-full">MongoDB</span>
              <span class="text-xs bg-blue-900 bg-opacity-50 px-2 py-1 rounded-full">IoT</span>
            </div>
            <div class="flex space-x-4">
              <a href="#" class="text-blue-400 hover:text-blue-300 transition-colors">
                <i class="fab fa-github mr-1"></i> Code
              </a>
              <a href="#" class="text-blue-400 hover:text-blue-300 transition-colors">
                <i class="fas fa-external-link-alt mr-1"></i> Demo
              </a>
            </div>
          </div>
        </div>
        
        <!-- Project 2 -->
        <div class="bg-white bg-opacity-5 rounded-xl overflow-hidden hover:transform hover:scale-105 transition-all duration-300">
          <div class="h-48 overflow-hidden">
            <img src="https://via.placeholder.com/600x400" alt="Project 2" class="w-full h-full object-cover" />
          </div>
          <div class="p-6">
            <h3 class="text-xl font-bold mb-2 text-blue-300">Construction Project Tracker</h3>
            <p class="text-gray-300 mb-4">
              A mobile application for tracking construction project progress, managing resources, and coordinating teams.
            </p>
            <div class="flex flex-wrap gap-2 mb-4">
              <span class="text-xs bg-blue-900 bg-opacity-50 px-2 py-1 rounded-full">React Native</span>
              <span class="text-xs bg-blue-900 bg-opacity-50 px-2 py-1 rounded-full">Firebase</span>
              <span class="text-xs bg-blue-900 bg-opacity-50 px-2 py-1 rounded-full">Redux</span>
              <span class="text-xs bg-blue-900 bg-opacity-50 px-2 py-1 rounded-full">Google Maps API</span>
            </div>
            <div class="flex space-x-4">
              <a href="#" class="text-blue-400 hover:text-blue-300 transition-colors">
                <i class="fab fa-github mr-1"></i> Code
              </a>
              <a href="#" class="text-blue-400 hover:text-blue-300 transition-colors">
                <i class="fas fa-external-link-alt mr-1"></i> Demo
              </a>
            </div>
          </div>
        </div>
        
        <!-- Project 3 -->
        <div class="bg-white bg-opacity-5 rounded-xl overflow-hidden hover:transform hover:scale-105 transition-all duration-300">
          <div class="h-48 overflow-hidden">
            <img src="https://via.placeholder.com/600x400" alt="Project 3" class="w-full h-full object-cover" />
          </div>
          <div class="p-6">
            <h3 class="text-xl font-bold mb-2 text-blue-300">Structural Analysis Tool</h3>
            <p class="text-gray-300 mb-4">
              A web-based tool for performing basic structural analysis and generating reports for small-scale projects.
            </p>
            <div class="flex flex-wrap gap-2 mb-4">
              <span class="text-xs bg-blue-900 bg-opacity-50 px-2 py-1 rounded-full">JavaScript</span>
              <span class="text-xs bg-blue-900 bg-opacity-50 px-2 py-1 rounded-full">Three.js</span>
              <span class="text-xs bg-blue-900 bg-opacity-50 px-2 py-1 rounded-full">WebGL</span>
              <span class="text-xs bg-blue-900 bg-opacity-50 px-2 py-1 rounded-full">Python</span>
            </div>
            <div class="flex space-x-4">
              <a href="#" class="text-blue-400 hover:text-blue-300 transition-colors">
                <i class="fab fa-github mr-1"></i> Code
              </a>
              <a href="#" class="text-blue-400 hover:text-blue-300 transition-colors">
                <i class="fas fa-external-link-alt mr-1"></i> Demo
              </a>
            </div>
          </div>
        </div>
      </div>
      
      <div class="text-center mt-12">
        <a href="https://github.com/yourusername" target="_blank" class="inline-block px-8 py-3 bg-white bg-opacity-10 rounded-full font-medium hover:bg-opacity-20 transition-all">
          <i class="fab fa-github mr-2"></i> View More on GitHub
        </a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'ProjectsSection'
}
</script>