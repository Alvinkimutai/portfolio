<template>
  <section id="education" class="py-20">
    <h2 class="section-title">Education</h2>
    
    <div class="max-w-4xl mx-auto grid md:grid-cols-2 gap-8">
      <!-- Education Item 1 -->
      <div class="bg-white bg-opacity-5 rounded-xl p-6 backdrop-filter backdrop-blur-sm hover:bg-opacity-10 transition-all">
        <div class="flex items-center mb-4">
          <div class="w-12 h-12 rounded-full bg-blue-900 flex items-center justify-center mr-4">
            <i class="fas fa-laptop-code text-xl"></i>
          </div>
          <div>
            <h3 class="text-xl font-bold text-blue-300">Master of Computer Science</h3>
            <p class="text-gray-300">University Name</p>
          </div>
        </div>
        <div class="flex justify-between items-center mb-4">
          <span class="text-sm bg-blue-900 bg-opacity-50 px-3 py-1 rounded-full">2020 - 2022</span>
          <span class="text-sm font-medium text-blue-300">GPA: 3.9/4.0</span>
        </div>
        <p class="text-gray-200">
          Specialized in software engineering and artificial intelligence. Completed coursework in advanced algorithms, 
          machine learning, and software architecture.
        </p>
      </div>
      
      <!-- Education Item 2 -->
      <div class="bg-white bg-opacity-5 rounded-xl p-6 backdrop-filter backdrop-blur-sm hover:bg-opacity-10 transition-all">
        <div class="flex items-center mb-4">
          <div class="w-12 h-12 rounded-full bg-blue-900 flex items-center justify-center mr-4">
            <i class="fas fa-building text-xl"></i>
          </div>
          <div>
            <h3 class="text-xl font-bold text-blue-300">Bachelor of Civil Engineering</h3>
            <p class="text-gray-300">University Name</p>
          </div>
        </div>
        <div class="flex justify-between items-center mb-4">
          <span class="text-sm bg-blue-900 bg-opacity-50 px-3 py-1 rounded-full">2014 - 2018</span>
          <span class="text-sm font-medium text-blue-300">GPA: 3.7/4.0</span>
        </div>
        <p class="text-gray-200">
          Focused on structural engineering and construction management. Participated in multiple design competitions 
          and completed a capstone project on sustainable building design.
        </p>
      </div>
      
      <!-- Certifications -->
      <div class="md:col-span-2 mt-8">
        <h3 class="text-2xl font-semibold mb-6 text-center text-blue-300">Certifications</h3>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
          <div class="bg-white bg-opacity-5 p-4 rounded-lg text-center hover:bg-opacity-10 transition-all">
            <i class="fas fa-certificate text-2xl mb-2 text-yellow-400"></i>
            <h4 class="font-medium">AWS Certified Developer</h4>
            <p class="text-sm text-gray-300">Amazon Web Services, 2023</p>
          </div>
          <div class="bg-white bg-opacity-5 p-4 rounded-lg text-center hover:bg-opacity-10 transition-all">
            <i class="fas fa-certificate text-2xl mb-2 text-yellow-400"></i>
            <h4 class="font-medium">Professional Engineer (PE)</h4>
            <p class="text-sm text-gray-300">State Board, 2020</p>
          </div>
          <div class="bg-white bg-opacity-5 p-4 rounded-lg text-center hover:bg-opacity-10 transition-all">
            <i class="fas fa-certificate text-2xl mb-2 text-yellow-400"></i>
            <h4 class="font-medium">Full Stack Web Development</h4>
            <p class="text-sm text-gray-300">Coding Bootcamp, 2021</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'ProfileEducation'
}
</script>