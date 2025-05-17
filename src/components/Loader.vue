<template>
  <div class="flex justify-center items-center">
    <div ref="spinner"></div>
  </div>
</template>

<script>
import { onMounted } from 'vue';
import { ring } from 'ldrs';

export default {
  name: 'LoaderSpinner',
  props: {
    color: {
      type: String,
      default: '#38bdf8'
    },
    size: {
      type: Number,
      default: 40
    }
  },
  setup(props) {
    onMounted(() => {
      // Register the spinner
      ring.register();
      
      // Create the spinner
      const spinner = document.createElement('l-ring');
      spinner.setAttribute('color', props.color);
      spinner.setAttribute('size', props.size);
      spinner.setAttribute('speed', '2');
      spinner.setAttribute('stroke', '5');
      
      // Add to the DOM
      document.querySelector('div[ref="spinner"]').appendChild(spinner);
    });
  }
}
</script>
