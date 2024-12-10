<script lang="ts">
  import { Link } from "svelte-routing";
</script>

<div class="bg-gradient-to-r from-primary-600 to-secondary-600">
  <div class="container mx-auto px-4 py-20 text-white">
    <div class="max-w-3xl">
      <h1 class="text-5xl font-bold mb-6">Empowering Lives Through Compassionate Care</h1>
      <p class="text-xl mb-8">Providing exceptional health and social care services to help individuals live their best lives.</p>
      <div class="flex space-x-4">
        <Link to="/services" class="btn bg-white text-primary-600 hover:bg-gray-200">
          Explore Services
        </Link>
        <Link to="/contact" class="btn border-2 border-white hover:bg-white hover:text-primary-600">
          Contact Us
        </Link>
      </div>
    </div>
  </div>
</div>

<section class="py-20">
  <div class="container mx-auto px-4">
    <h2 class="text-3xl font-bold text-center mb-12">Our Services</h2>
    <div class="grid md:grid-cols-3 gap-8">
      <div class="bg-white p-6 rounded-lg shadow-lg">
        <h3 class="text-xl font-semibold mb-4">Supported Accommodation</h3>
        <p class="text-gray-600">Helping individuals maintain independence while receiving necessary support.</p>
      </div>
      <div class="bg-white p-6 rounded-lg shadow-lg">
        <h3 class="text-xl font-semibold mb-4">Residential Care</h3>
        <p class="text-gray-600">24/7 professional care in a comfortable, home-like environment.</p>
      </div>
      <div class="bg-white p-6 rounded-lg shadow-lg">
        <h3 class="text-xl font-semibold mb-4">Specialist Care</h3>
        <p class="text-gray-600">Tailored care solutions for complex needs and requirements.</p>
      </div>
    </div>
  </div>
</section>

<section class="bg-gray-50 py-20">
  <div class="container mx-auto px-4">
    <h2 class="text-3xl font-bold text-center mb-12">Why Choose Pillarays?</h2>
    <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
      <div class="text-center">
        <div class="text-primary-600 text-4xl mb-4">20+</div>
        <p class="font-semibold">Years Experience</p>
      </div>
      <div class="text-center">
        <div class="text-primary-600 text-4xl mb-4">500+</div>
        <p class="font-semibold">Clients Supported</p>
      </div>
      <div class="text-center">
        <div class="text-primary-600 text-4xl mb-4">100%</div>
        <p class="font-semibold">Qualified Staff</p>
      </div>
      <div class="text-center">
        <div class="text-primary-600 text-4xl mb-4">24/7</div>
        <p class="font-semibold">Support Available</p>
      </div>
    </div>
  </div>
</section>

