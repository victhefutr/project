<script lang="ts">
  import { Link } from "svelte-routing";
</script>

<footer class="bg-gray-900 text-white">
  <div class="container mx-auto px-4 py-12">
    <div class="grid md:grid-cols-4 gap-8">
      <div>
        <h3 class="text-xl font-bold mb-4">Pillarays</h3>
        <p class="text-gray-400">Empowering lives through compassionate care and support.</p>
      </div>
      <div>
        <h4 class="font-semibold mb-4">Quick Links</h4>
        <ul class="space-y-2">
          <li><Link to="/services" class="text-gray-400 hover:text-white">Services</Link></li>
          <li><Link to="/about" class="text-gray-400 hover:text-white">About Us</Link></li>
          <li><Link to="/contact" class="text-gray-400 hover:text-white">Contact</Link></li>
          <li><Link to="/foundation" class="text-gray-400 hover:text-white">Foundation</Link></li>
        </ul>
      </div>
      <div>
        <h4 class="font-semibold mb-4">Contact</h4>
        <ul class="space-y-2 text-gray-400">
          <li>123 Care Street</li>
          <li>London, UK</li>
          <li>Phone: (123) 456-7890</li>
          <li>Email: info@pillarays.com</li>
        </ul>
      </div>
      <div>
        <h4 class="font-semibold mb-4">Follow Us</h4>
        <div class="flex space-x-4">
          <a href="#" class="text-gray-400 hover:text-white">
            <span class="sr-only">Facebook</span>
            <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24">
              <path d="M18.77,7.46H14.5v-1.9c0-.9.6-1.1,1-1.1h3V.5h-4.33C10.24.5,9.5,3.44,9.5,5.32v2.15h-3v4h3v12h5v-12h3.85l.42-4Z"/>
            </svg>
          </a>
          <a href="#" class="text-gray-400 hover:text-white">
            <span class="sr-only">Twitter</span>
            <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24">
              <path d="M23.953 4.57a10 10 0 01-2.825.775 4.958 4.958 0 002.163-2.723c-.951.555-2.005.959-3.127 1.184a4.92 4.92 0 00-8.384 4.482C7.69 8.095 4.067 6.13 1.64 3.162a4.822 4.822 0 00-.666 2.475c0 1.71.87 3.213 2.188 4.096a4.904 4.904 0 01-2.228-.616v.06a4.923 4.923 0 003.946 4.827 4.996 4.996 0 01-2.212.085 4.936 4.936 0 004.604 3.417 9.867 9.867 0 01-6.102 2.105c-.39 0-.779-.023-1.17-.067a13.995 13.995 0 007.557 2.209c9.053 0 13.998-7.496 13.998-13.985 0-.21 0-.42-.015-.63A9.935 9.935 0 0024 4.59z"/>
            </svg>
          </a>
          <a href="#" class="text-gray-400 hover:text-white">
            <span class="sr-only">LinkedIn</span>
            <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24">
              <path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/>
            </svg>
          </a>
        </div>
      </div>
    </div>
    <div class="border-t border-gray-800 mt-8 pt-8 text-center text-gray-400">
      <p>&copy; {new Date().getFullYear()} Pillarays. All rights reserved.</p>
    </div>
  </div>
</footer>