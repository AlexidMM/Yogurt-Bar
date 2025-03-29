<!-- src/routes/+page.svelte -->
<script lang="ts">
	import { page } from "$app/state";
    let companyName = "YoQui";
</script>

<nav class="flex justify-between items-center p-4 bg-pink-50 text-gray-800 shadow-sm">
  <h1 class="text-2xl font-semibold tracking-wide">{companyName}</h1>
  <div class="space-x-4">
    <button class="px-5 py-2 bg-white text-gray-800 rounded-md shadow-sm hover:bg-pink-100 transition border border-pink-200">
      Productos
    </button>
    <button class="px-5 py-2 bg-white text-gray-800 rounded-md shadow-sm hover:bg-pink-100 transition border border-pink-200">
      Ubicaciones
    </button>
  </div>
</nav>

<main class="flex flex-col items-center min-h-screen bg-pink-50 text-gray-800">
  <!-- Hero Banner -->
  <section class="w-full max-w-6xl px-4 py-12">
    <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
      <div class="flex flex-col justify-center">
        <h2 class="text-4xl font-bold text-gray-800">Descubre nuestro delicioso mundo de yogurt</h2>
        <p class="mt-4 text-gray-600 text-lg">
          Un equilibrio perfecto entre suavidad y frescura, con ingredientes naturales y un sabor irresistible.
        </p>
        <button class="mt-6 px-6 py-3 bg-pink-400 text-white rounded-md shadow-md text-lg hover:bg-pink-500 transition w-max">
          ¡Ordena ahora!
        </button>
      </div>
      <div class="flex justify-center items-center">
        <img src="/yogurt-bar.jpg" alt="Barrita de yogurt" class="rounded-lg shadow-lg w-full max-w-md h-auto object-cover">
      </div>
    </div>
  </section>
  
  <!-- Product Grid -->
  <section class="w-full max-w-6xl px-4 py-8 mb-12">
    <h3 class="text-2xl font-semibold mb-8 text-center">Nuestras Especialidades</h3>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
      <!-- Product Card 1 -->
      <div class="bg-white rounded-lg overflow-hidden shadow-md hover:shadow-lg transition">
        <div class="p-1 bg-pink-100">
          <p class="text-sm text-pink-600 font-medium">5 variedades</p>
        </div>
        <div class="p-6">
          <h4 class="text-xl font-bold mb-2">YOGURT CLÁSICO</h4>
          <p class="text-gray-600 mb-4">Nuestra receta original con ingredientes premium y textura perfecta.</p>
          <button class="text-pink-500 font-medium hover:text-pink-600 transition">Leer Más</button>
        </div>
      </div>
      
      <!-- Product Card 2 -->
      <div class="bg-white rounded-lg overflow-hidden shadow-md hover:shadow-lg transition">
        <div class="p-1 bg-pink-100">
          <p class="text-sm text-pink-600 font-medium">5 variedades</p>
        </div>
        <div class="p-6">
          <h4 class="text-xl font-bold mb-2">YOGURT FRUTAL</h4>
          <p class="text-gray-600 mb-4">Combinación perfecta de yogurt cremoso con frutas frescas de temporada.</p>
          <button class="text-pink-500 font-medium hover:text-pink-600 transition">Leer Más</button>
        </div>
      </div>
      
      <!-- Product Card 3 -->
      <div class="bg-white rounded-lg overflow-hidden shadow-md hover:shadow-lg transition">
        <div class="p-1 bg-pink-100">
          <p class="text-sm text-pink-600 font-medium">5 variedades</p>
        </div>
        <div class="p-6">
          <h4 class="text-xl font-bold mb-2">TOPPINGS PREMIUM</h4>
          <p class="text-gray-600 mb-4">Complementa tu yogurt con nuestra selección de toppings artesanales.</p>
          <button class="text-pink-500 font-medium hover:text-pink-600 transition">Leer Más</button>
        </div>
      </div>
    </div>
  </section>
</main>

<footer class="bg-white py-6 border-t border-pink-100">
  <div class="container mx-auto text-center text-gray-600">
    <p>&copy; 2025 {companyName}. Todos los derechos reservados.</p>
  </div>
</footer>