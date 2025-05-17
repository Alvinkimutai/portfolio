<template>
  <section id="contact" class="py-20">
    <h2 class="section-title">Get In Touch</h2>
    
    <div class="max-w-4xl mx-auto">
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <!-- Contact Form -->
        <div class="bg-white bg-opacity-5 p-8 rounded-xl backdrop-filter backdrop-blur-sm">
          <h3 class="text-2xl font-semibold mb-6 text-blue-300">Send Me a Message</h3>
          <form @submit.prevent="submitForm">
            <div class="mb-4">
              <label for="name" class="block text-sm font-medium mb-2">Name</label>
              <input 
                type="text" 
                id="name" 
                v-model="form.name" 
                class="w-full px-4 py-2 bg-white bg-opacity-10 border border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500"
                required
              />
            </div>
            <div class="mb-4">
              <label for="email" class="block text-sm font-medium mb-2">Email</label>
              <input 
                type="email" 
                id="email" 
                v-model="form.email" 
                class="w-full px-4 py-2 bg-white bg-opacity-10 border border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500"
                required
              />
            </div>
            <div class="mb-4">
              <label for="subject" class="block text-sm font-medium mb-2">Subject</label>
              <input 
                type="text" 
                id="subject" 
                v-model="form.subject" 
                class="w-full px-4 py-2 bg-white bg-opacity-10 border border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500"
                required
              />
            </div>
            <div class="mb-6">
              <label for="message" class="block text-sm font-medium mb-2">Message</label>
              <textarea 
                id="message" 
                v-model="form.message" 
                rows="5" 
                class="w-full px-4 py-2 bg-white bg-opacity-10 border border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500"
                required
              ></textarea>
            </div>
            <button 
              type="submit" 
              class="w-full py-3 bg-gradient-to-r from-blue-500 to-purple-600 rounded-lg font-medium hover:opacity-90 transition-opacity"
              :disabled="isSubmitting"
            >
              {{ isSubmitting ? 'Sending...' : 'Send Message' }}
            </button>
          </form>
        </div>
        
        <!-- Contact Information -->
        <div>
          <div class="bg-white bg-opacity-5 p-8 rounded-xl backdrop-filter backdrop-blur-sm mb-8">
            <h3 class="text-2xl font-semibold mb-6 text-blue-300">Contact Information</h3>
            <div class="space-y-4">
              <div class="flex items-center">
                <div class="w-10 h-10 rounded-full bg-blue-900 flex items-center justify-center mr-4">
                  <i class="fas fa-envelope"></i>
                </div>
                <div>
                  <p class="text-sm text-gray-300">Email</p>
                  <a href="mailto:your.email@example.com" class="text-blue-300 hover:text-blue-200">your.email@example.com</a>
                </div>
              </div>
              <div class="flex items-center">
                <div class="w-10 h-10 rounded-full bg-blue-900 flex items-center justify-center mr-4">
                  <i class="fas fa-phone"></i>
                </div>
                <div>
                  <p class="text-sm text-gray-300">Phone</p>
                  <a href="tel:+1234567890" class="text-blue-300 hover:text-blue-200">+1 (234) 567-890</a>
                </div>
              </div>
              <div class="flex items-center">
                <div class="w-10 h-10 rounded-full bg-blue-900 flex items-center justify-center mr-4">
                  <i class="fas fa-map-marker-alt"></i>
                </div>
                <div>
                  <p class="text-sm text-gray-300">Location</p>
                  <p>City, Country</p>
                </div>
              </div>
            </div>
          </div>
          
          <!-- Social Links -->
          <div class="bg-white bg-opacity-5 p-8 rounded-xl backdrop-filter backdrop-blur-sm">
            <h3 class="text-2xl font-semibold mb-6 text-blue-300">Connect With Me</h3>
            <div class="flex space-x-4">
              <a href="#" class="w-12 h-12 rounded-full bg-blue-900 flex items-center justify-center hover:bg-blue-800 transition-colors">
                <i class="fab fa-linkedin-in"></i>
              </a>
              <a href="#" class="w-12 h-12 rounded-full bg-blue-900 flex items-center justify-center hover:bg-blue-800 transition-colors">
                <i class="fab fa-github"></i>
              </a>
              <a href="#" class="w-12 h-12 rounded-full bg-blue-900 flex items-center justify-center hover:bg-blue-800 transition-colors">
                <i class="fab fa-twitter"></i>
              </a>
              <a href="#" class="w-12 h-12 rounded-full bg-blue-900 flex items-center justify-center hover:bg-blue-800 transition-colors">
                <i class="fab fa-dev"></i>
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'ProfileContact',
  data() {
    return {
      form: {
        name: '',
        email: '',
        subject: '',
        message: ''
      },
      isSubmitting: false
    }
  },
  methods: {
    submitForm() {
      this.isSubmitting = true;
      
      // Simulate form submission
      setTimeout(() => {
        alert('Thank you for your message! This is a demo form - in a real portfolio, this would send an email.');
        this.form = {
          name: '',
          email: '',
          subject: '',
          message: ''
        };
        this.isSubmitting = false;
      }, 1500);
      
      // In a real application, you would send the form data to a backend service
      // Example:
      // fetch('/api/contact', {
      //   method: 'POST',
      //   headers: {
      //     'Content-Type': 'application/json',
      //   },
      //   body: JSON.stringify(this.form),
      // })
      // .then(response => response.json())
      // .then(data => {
      //   // Handle success
      //   this.isSubmitting = false;
      // })
      // .catch(error => {
      //   // Handle error
      //   this.isSubmitting = false;
      // });
    }
  }
}
</script>