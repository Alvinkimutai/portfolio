<template>
  <div class="bg-white bg-opacity-5 rounded-lg p-6 backdrop-filter backdrop-blur-sm hover:bg-opacity-10 transition-all">
    <div class="flex flex-col items-center">
      <div class="text-4xl mb-4">
        <i :class="icon"></i>
      </div>
      <h4 class="text-lg font-medium mb-3">{{ title }}</h4>
      <div class="w-full bg-gray-700 rounded-full h-2.5">
        <div class="bg-gradient-to-r from-blue-500 to-purple-600 h-2.5 rounded-full" :style="{ width: `${level}%` }"></div>
      </div>
      <span class="mt-2 text-sm text-gray-300">{{ level }}%</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SkillCard',
  props: {
    title: {
      type: String,
      required: true
    },
    icon: {
      type: String,
      required: true
    },
    level: {
      type: Number,
      required: true,
      validator: value => value >= 0 && value <= 100
    }
  }
}
</script>