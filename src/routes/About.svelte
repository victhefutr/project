<script lang="ts">
  const team = [
    {
      name: "Sarah Johnson",
      role: "Chief Executive Officer",
      image: "https://images.unsplash.com/photo-1494790108377-be9c29b29330"
    },
    {
      name: "Michael Chen",
      role: "Head of Care Services",
      image: "https://images.unsplash.com/photo-1472099645785-5658abf4ff4e"
    },
    {
      name: "Emma Williams",
      role: "Clinical Director",
      image: "https://images.unsplash.com/photo-1438761681033-6461ffad8d80"
    }
  ];
</script>

<div class="py-12">
  <div class="container">
    <div class="max-w-3xl mx-auto text-center mb-16">
      <h1 class="text-4xl font-bold mb-6">About Pillarays</h1>
      <p class="text-xl text-gray-600">Dedicated to providing exceptional care and support services that enhance the quality of life for our clients.</p>
    </div>

    <div class="grid md:grid-cols-2 gap-12 mb-16">
      <div>
        <h2 class="text-2xl font-bold mb-4">Our Mission</h2>
        <p class="text-gray-600 mb-4">To empower individuals through compassionate care, promoting independence and dignity while ensuring the highest standards of support.</p>
        <ul class="space-y-2 text-gray-600">
          <li class="flex items-center">
            <svg class="w-5 h-5 text-primary-500 mr-2" fill="currentColor" viewBox="0 0 20 20">
              <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
            </svg>
            Person-centered care approach
          </li>
          <li class="flex items-center">
            <svg class="w-5 h-5 text-primary-500 mr-2" fill="currentColor" viewBox="0 0 20 20">
              <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
            </svg>
            Professional development
          </li>
          <li class="flex items-center">
            <svg class="w-5 h-5 text-primary-500 mr-2" fill="currentColor" viewBox="0 0 20 20">
              <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
            </svg>
            Community integration
          </li>
        </ul>
      </div>
      <div>
        <h2 class="text-2xl font-bold mb-4">Our Values</h2>
        <p class="text-gray-600 mb-4">We are guided by core values that ensure we deliver the best possible care:</p>
        <ul class="space-y-2 text-gray-600">
          <li class="flex items-center">
            <svg class="w-5 h-5 text-primary-500 mr-2" fill="currentColor" viewBox="0 0 20 20">
              <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
            </svg>
            Respect and dignity
          </li>
          <li class="flex items-center">
            <svg class="w-5 h-5 text-primary-500 mr-2" fill="currentColor" viewBox="0 0 20 20">
              <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
            </svg>
            Excellence in care
          </li>
          <li class="flex items-center">
            <svg class="w-5 h-5 text-primary-500 mr-2" fill="currentColor" viewBox="0 0 20 20">
              <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
            </svg>
            Continuous improvement
          </li>
        </ul>
      </div>
    </div>

    <h2 class="text-3xl font-bold text-center mb-12">Our Leadership Team</h2>
    <div class="grid md:grid-cols-3 gap-8">
      {#each team as member}
        <div class="text-center">
          <img src={member.image} alt={member.name} class="w-32 h-32 rounded-full mx-auto mb-4 object-cover">
          <h3 class="text-xl font-semibold">{member.name}</h3>
          <p class="text-gray-600">{member.role}</p>
        </div>
      {/each}
    </div>
  </div>
</div>