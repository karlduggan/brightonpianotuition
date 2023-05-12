<template>
    <div class="container mx-auto py-8">
      <h1 class="text-3xl md:text-4xl font-bold mb-8">Contact Us</h1>
      <div class="flex flex-col md:flex-row justify-between">
        <div class="w-full md:w-1/2 mb-8 md:mb-0">
          <h2 class="text-xl md:text-2xl font-bold mb-4">Get in Touch</h2>
          <p class="mb-4">Have a question? Want to book a lesson? We'd love to hear from you! Fill out the form below and we'll get back to you as soon as possible.</p>
          <form class="w-full" @submit.prevent="submitForm">
            <div class="flex flex-col mb-4">
              <label for="name" class="font-bold mb-2">Name:</label>
              <input type="text" id="name" name="name" class="border py-2 px-3" v-model="form.name" required>
            </div>
            <div class="flex flex-col mb-4">
              <label for="email" class="font-bold mb-2">Email:</label>
              <input type="email" id="email" name="email" class="border py-2 px-3" v-model="form.email" required>
            </div>
            <div class="flex flex-col mb-4">
              <label for="message" class="font-bold mb-2">Message:</label>
              <textarea id="message" name="message" class="border py-2 px-3 h-32" v-model="form.message" required></textarea>
            </div>
            <button type="submit" class="bg-blue-500 text-white py-2 px-4 rounded hover:bg-blue-600">Submit</button>
          </form>
        </div>
        <div class="w-full md:w-1/2">
          <h2 class="text-xl md:text-2xl font-bold mb-4">Find Us</h2>
          <p class="mb-4">We're located in the heart of Brighton, just a short walk from the train station.</p>
          <div class="mb-4">
            <h3 class="font-bold mb-2">Address:</h3>
            <p>123 Main St</p>
            <p>Brighton, BN1 1AB</p>
          </div>
          <div class="mb-4">
            <h3 class="font-bold mb-2">Phone:</h3>
            <p>01273 123456</p>
          </div>
          <div class="mb-4">
            <h3 class="font-bold mb-2">Email:</h3>
            <p>info@brightonpianotuition.com</p>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        form: {
          name: '',
          email: '',
          message: ''
        }
      }
    },
    methods: {
      submitForm() {
        // Send form data to server using axios or fetch
        console.log(this.form)
      }
    }
  }
  </script>
  