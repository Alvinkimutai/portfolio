<template>
  <section id="about" class="py-20">
    <h2 class="section-title">About Me</h2>
    <div class="max-w-4xl mx-auto bg-white bg-opacity-5 p-8 rounded-xl backdrop-filter backdrop-blur-sm">
      <div class="flex flex-col md:flex-row gap-8 items-center">
        <div class="md:w-1/3">
          <!-- Replace with your actual image -->
          <div class="w-64 h-64 rounded-full overflow-hidden mx-auto border-4 border-blue-400">
            <img src="https://media.licdn.com/dms/image/v2/C4E22AQGfMGvMBEcqyQ/feedshare-shrink_2048_1536/feedshare-shrink_2048_1536/0/1634668334200?e=2147483647&v=beta&t=zoTfzvsDbj_bdgCDZrVtJBDQ2cBwfHUSKan46XlqevI" />
          </div>
        </div>
        <div class="md:w-2/3">
          <p class="text-lg mb-4">
            Hello! I'm a passionate professional with expertise in both software development and civil engineering. 
            My unique background allows me to bridge the gap between technical software solutions and real-world engineering challenges.
          </p>
          <p class="text-lg mb-4">
            With experience in various programming languages and engineering principles, I enjoy creating innovative solutions 
            that combine the best of both worlds. I'm particularly interested in how technology can improve infrastructure design and management.
          </p>
          <p class="text-lg">
            When I'm not coding or designing structures, you can find me [your hobbies/interests]. I'm always eager to learn new technologies 
            and methodologies to enhance my skill set and deliver better results.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'ProfileAbout'
}
</script>