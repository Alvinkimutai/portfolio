<template>
  <section id="skills" class="py-20">
    <h2 class="section-title">My Skills</h2>
    
    <div class="max-w-6xl mx-auto">
      <!-- Software Development Skills -->
      <div class="mb-16">
        <h3 class="text-2xl font-semibold mb-6 text-center text-blue-300">Software Development</h3>
        <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6">
          <SkillCard title="JavaScript" icon="devicon-javascript-plain colored" :level="90" />
          <SkillCard title="Vue.js" icon="devicon-vuejs-plain colored" :level="85" />
          <SkillCard title="React" icon="devicon-react-original colored" :level="80" />
          <SkillCard title="Node.js" icon="devicon-nodejs-plain colored" :level="75" />
          <SkillCard title="Python" icon="devicon-python-plain colored" :level="85" />
          <SkillCard title="Java" icon="devicon-java-plain colored" :level="70" />
          <SkillCard title="C#" icon="devicon-csharp-plain colored" :level="65" />
          <SkillCard title="SQL" icon="devicon-mysql-plain colored" :level="80" />
        </div>
      </div>
      
      <!-- Civil Engineering Skills -->
      <div>
        <h3 class="text-2xl font-semibold mb-6 text-center text-blue-300">Civil Engineering</h3>
        <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6">
          <SkillCard title="Structural Analysis" icon="fas fa-building" :level="90" />
          <SkillCard title="AutoCAD" icon="fas fa-drafting-compass" :level="85" />
          <SkillCard title="Revit" icon="fas fa-cube" :level="75" />
          <SkillCard title="Project Management" icon="fas fa-tasks" :level="80" />
          <SkillCard title="Construction Planning" icon="fas fa-hard-hat" :level="85" />
          <SkillCard title="Material Testing" icon="fas fa-vial" :level="70" />
          <SkillCard title="Surveying" icon="fas fa-mountain" :level="75" />
          <SkillCard title="Environmental Engineering" icon="fas fa-leaf" :level="65" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import SkillCard from './SkillCard.vue'

export default {
  name: 'SkillsSection',
  components: {
    SkillCard
  }
}
</script>