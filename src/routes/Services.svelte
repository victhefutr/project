<script lang="ts">
  import { Link } from "svelte-routing";

  const services = [
    {
      title: "Supported Accommodation",
      description: "Independent living with personalized support tailored to individual needs. Our supported accommodation services help residents maintain autonomy while receiving necessary assistance.",
      features: ["24/7 Support Staff", "Individual Care Plans", "Life Skills Development", "Community Integration"]
    },
    {
      title: "Residential Care",
      description: "Professional care in a comfortable, home-like environment. Our residential care homes provide comprehensive support for those requiring regular assistance.",
      features: ["Round-the-clock Care", "Medical Support", "Social Activities", "Nutritious Meals"]
    },
    {
      title: "Specialist Care",
      description: "Specialized support for complex needs, including learning disabilities, mental health, and physical disabilities.",
      features: ["Specialized Staff", "Therapeutic Support", "Behavioral Support", "Personal Care"]
    },
    {
      title: "Respite Care",
      description: "Short-term care providing relief for primary caregivers and families while maintaining quality care for loved ones.",
      features: ["Flexible Duration", "Emergency Support", "Professional Care", "Activities Program"]
    }
  ];
</script>

<div class="py-12 bg-gray-50">
  <div class="container">
    <h1 class="text-4xl font-bold text-center mb-12">Our Services</h1>
    
    <div class="space-y-12">
      {#each services as service}
        <div class="bg-white rounded-lg shadow-lg overflow-hidden">
          <div class="p-8">
            <h2 class="text-2xl font-bold text-primary-600 mb-4">{service.title}</h2>
            <p class="text-gray-600 mb-6">{service.description}</p>
            <div class="grid md:grid-cols-2 gap-4">
              {#each service.features as feature}
                <div class="flex items-center space-x-2">
                  <svg class="w-5 h-5 text-primary-500" fill="currentColor" viewBox="0 0 20 20">
                    <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
                  </svg>
                  <span class="text-gray-700">{feature}</span>
                </div>
              {/each}
            </div>
          </div>
        </div>
      {/each}
    </div>

    <div class="mt-12 text-center">
      <Link to="/contact" class="btn btn-primary">
        Discuss Your Care Needs
      </Link>
    </div>
  </div>
</div>