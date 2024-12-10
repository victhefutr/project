<script lang="ts">
  const initiatives = [
    {
      title: "Community Support Programs",
      description: "Supporting local communities through various outreach programs and initiatives.",
      image: "https://images.unsplash.com/photo-1559027615-cd4628902d4a"
    },
    {
      title: "Education & Training",
      description: "Providing educational resources and training for caregivers and healthcare professionals.",
      image: "https://images.unsplash.com/photo-1524178232363-1fb2b075b655"
    },
    {
      title: "Research & Innovation",
      description: "Investing in research to improve care practices and develop innovative solutions.",
      image: "https://images.unsplash.com/photo-1576091160399-112ba8d25d1d"
    }
  ];
</script>

<div class="py-12">
  <div class="container">
    <div class="max-w-3xl mx-auto text-center mb-16">
      <h1 class="text-4xl font-bold mb-6">Pillarays Foundation</h1>
      <p class="text-xl text-gray-600">Making a difference in healthcare and social care through innovation, education, and community support.</p>
    </div>

    <div class="grid md:grid-cols-3 gap-8 mb-16">
      {#each initiatives as initiative}
        <div class="bg-white rounded-lg shadow-lg overflow-hidden">
          <img src={initiative.image} alt={initiative.title} class="w-full h-48 object-cover">
          <div class="p-6">
            <h3 class="text-xl font-bold mb-2">{initiative.title}</h3>
            <p class="text-gray-600">{initiative.description}</p>
          </div>
        </div>
      {/each}
    </div>

    <div class="bg-primary-50 rounded-lg p-8 mb-16">
      <div class="max-w-3xl mx-auto text-center">
        <h2 class="text-2xl font-bold mb-4">Get Involved</h2>
        <p class="text-gray-600 mb-8">Join us in our mission to improve healthcare and social care services. Whether through volunteering, donations, or partnerships, your support makes a difference.</p>
        <div class="flex justify-center space-x-4">
          <button class="btn btn-primary">Donate Now</button>
          <button class="btn btn-secondary">Volunteer</button>
        </div>
      </div>
    </div>

    <div class="grid md:grid-cols-2 gap-12">
      <div>
        <h2 class="text-2xl font-bold mb-6">Our Impact</h2>
        <div class="space-y-4">
          <div class="flex items-center space-x-4">
            <div class="flex-shrink-0 w-12 h-12 bg-primary-100 rounded-full flex items-center justify-center">
              <span class="text-primary-600 font-bold">1K+</span>
            </div>
            <div>
              <h3 class="font-semibold">People Supported</h3>
              <p class="text-gray-600">Through our community programs</p>
            </div>
          </div>
          <div class="flex items-center space-x-4">
            <div class="flex-shrink-0 w-12 h-12 bg-primary-100 rounded-full flex items-center justify-center">
              <span class="text-primary-600 font-bold">50+</span>
            </div>
            <div>
              <h3 class="font-semibold">Partner Organizations</h3>
              <p class="text-gray-600">Working together for better care</p>
            </div>
          </div>
          <div class="flex items-center space-x-4">
            <div class="flex-shrink-0 w-12 h-12 bg-primary-100 rounded-full flex items-center justify-center">
              <span class="text-primary-600 font-bold">10+</span>
            </div>
            <div>
              <h3 class="font-semibold">Research Projects</h3>
              <p class="text-gray-600">Advancing care practices</p>
            </div>
          </div>
        </div>
      </div>
      <div>
        <h2 class="text-2xl font-bold mb-6">Latest News</h2>
        <div class="space-y-6">
          <div class="border-l-4 border-primary-500 pl-4">
            <h3 class="font-semibold">New Training Program Launched</h3>
            <p class="text-gray-600">Supporting healthcare professionals with advanced care techniques.</p>
            <p class="text-sm text-gray-500">March 15, 2024</p>
          </div>
          <div class="border-l-4 border-primary-500 pl-4">
            <h3 class="font-semibold">Community Partnership Success</h3>
            <p class="text-gray-600">Celebrating the success of our latest community initiative.</p>
            <p class="text-sm text-gray-500">March 1, 2024</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>