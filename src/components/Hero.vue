<template>
  <section class="pt-32 pb-20 flex flex-col items-center justify-center text-center">
    <div class="max-w-3xl mx-auto">
      <h1 class="text-5xl md:text-6xl font-bold mb-6">
        <span class="bg-clip-text text-transparent bg-gradient-to-r from-blue-400 to-purple-500">
          Alvin Kimutai
        </span>
      </h1>
      <h2 class="text-2xl md:text-3xl mb-8">Software Developer & Civil Engineer</h2>
      <p class="text-lg md:text-xl mb-10 text-gray-200">
        Building innovative solutions at the intersection of software development and civil engineering
      </p>
      <div class="flex flex-wrap justify-center gap-4">
        <a href="#contact" class="px-8 py-3 bg-gradient-to-r from-blue-500 to-purple-600 rounded-full font-medium hover:opacity-90 transition-opacity">
          Contact Me
        </a>
        <a href="#projects" class="px-8 py-3 bg-white bg-opacity-10 rounded-full font-medium hover:bg-opacity-20 transition-all">
          View Projects
        </a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'HeroSection'
}
</script>