<script lang="ts">
  let formData = {
    name: '',
    email: '',
    phone: '',
    message: ''
  };

  function handleSubmit() {
    // Handle form submission
    console.log('Form submitted:', formData);
  }
</script>

<div class="py-12 bg-gray-50">
  <div class="container">
    <div class="max-w-4xl mx-auto">
      <h1 class="text-4xl font-bold text-center mb-12">Contact Us</h1>

      <div class="grid md:grid-cols-2 gap-12">
        <div>
          <h2 class="text-2xl font-bold mb-6">Get in Touch</h2>
          <div class="space-y-6">
            <div class="flex items-start space-x-4">
              <div class="flex-shrink-0">
                <svg class="w-6 h-6 text-primary-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"/>
                </svg>
              </div>
              <div>
                <h3 class="font-semibold">Phone</h3>
                <p class="text-gray-600">(123) 456-7890</p>
              </div>
            </div>

            <div class="flex items-start space-x-4">
              <div class="flex-shrink-0">
                <svg class="w-6 h-6 text-primary-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/>
                </svg>
              </div>
              <div>
                <h3 class="font-semibold">Email</h3>
                <p class="text-gray-600">info@pillarays.com</p>
              </div>
            </div>

            <div class="flex items-start space-x-4">
              <div class="flex-shrink-0">
                <svg class="w-6 h-6 text-primary-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"/>
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"/>
                </svg>
              </div>
              <div>
                <h3 class="font-semibold">Address</h3>
                <p class="text-gray-600">123 Care Street<br>London, UK</p>
              </div>
            </div>
          </div>
        </div>

        <div class="bg-white rounded-lg shadow-lg p-8">
          <h2 class="text-2xl font-bold mb-6">Send us a Message</h2>
          <form on:submit|preventDefault={handleSubmit} class="space-y-6">
            <div>
              <label for="name" class="block text-sm font-medium text-gray-700">Name</label>
              <input
                type="text"
                id="name"
                bind:value={formData.name}
                class="mt-1 block w-full rounded-md border-gray-300 shadow-sm focus:border-primary-500 focus:ring-primary-500"
                required
              >
            </div>

            <div>
              <label for="email" class="block text-sm font-medium text-gray-700">Email</label>
              <input
                type="email"
                id="email"
                bind:value={formData.email}
                class="mt-1 block w-full rounded-md border-gray-300 shadow-sm focus:border-primary-500 focus:ring-primary-500"
                required
              >
            </div>

            <div>
              <label for="phone" class="block text-sm font-medium text-gray-700">Phone</label>
              <input
                type="tel"
                id="phone"
                bind:value={formData.phone}
                class="mt-1 block w-full rounded-md border-gray-300 shadow-sm focus:border-primary-500 focus:ring-primary-500"
              >
            </div>

            <div>
              <label for="message" class="block text-sm font-medium text-gray-700">Message</label>
              <textarea
                id="message"
                bind:value={formData.message}
                rows="4"
                class="mt-1 block w-full rounded-md border-gray-300 shadow-sm focus:border-primary-500 focus:ring-primary-500"
                required
              ></textarea>
            </div>

            <button type="submit" class="btn btn-primary w-full">
              Send Message
            </button>
          </form>
        </div>
      </div>
    </div>
  </div>
</div>