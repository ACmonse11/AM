<template>
  <!-- NAVBAR -->
  <header class="fixed top-0 left-0 w-full z-40 bg-black/30 backdrop-blur-xl border-b border-white/10">
    <nav class="max-w-7xl mx-auto px-6 py-4 flex items-center justify-between">
      <h1 class="text-2xl font-extrabold tracking-tight text-emerald-400">Athletix</h1>

      <ul class="hidden md:flex items-center gap-8 text-gray-300 font-medium">
        <li><a href="#features" class="hover:text-white transition">Características</a></li>
        <li><a href="#programs" class="hover:text-white transition">Programas</a></li>
        <li><a href="#reviews" class="hover:text-white transition">Reseñas</a></li>
      </ul>

      <button
        class="px-6 py-2 rounded-full border border-gray-600 text-gray-200 hover:bg-emerald-400 hover:text-black transition font-semibold">
        Iniciar
      </button>
    </nav>
  </header>

  <!-- HERO -->
  <section class="min-h-screen flex items-center bg-gradient-to-br from-black via-gray-900 to-gray-800 pt-24">
    <div class="max-w-7xl mx-auto px-6 grid md:grid-cols-2 gap-14 items-center">

      <!-- Text -->
      <div>
        <h2 class="text-5xl md:text-6xl font-extrabold text-white leading-tight">
          Eleva tu rendimiento,
          <span class="text-emerald-400">sin límites</span>
        </h2>

        <p class="text-gray-300 mt-6 text-lg leading-relaxed max-w-lg">
          Athletix combina ciencia del deporte, IA y estadísticas avanzadas para ayudarte a entrenar de manera
          inteligente y alcanzar tu máximo potencial.
        </p>

        <div class="mt-8 flex gap-4">
          <button class="px-7 py-3 bg-emerald-400 text-black rounded-lg font-bold shadow-lg hover:bg-emerald-300 transition">
            Empezar gratis
          </button>

          <button class="px-7 py-3 border border-gray-500 rounded-lg text-white hover:bg-gray-700 transition">
            Ver más
          </button>
        </div>

        <!-- Stats -->
        <div class="flex gap-10 mt-12">
          <div>
            <p class="text-3xl font-extrabold text-emerald-400">+85K</p>
            <span class="text-gray-400 text-sm">Usuarios activos</span>
          </div>

          <div>
            <p class="text-3xl font-extrabold text-emerald-400">150+</p>
            <span class="text-gray-400 text-sm">Rutinas únicas</span>
          </div>

          <div>
            <p class="text-3xl font-extrabold text-emerald-400">4.9★</p>
            <span class="text-gray-400 text-sm">Valoración global</span>
          </div>
        </div>
      </div>

      <!-- Card -->
      <div
        class="p-6 rounded-3xl bg-white/5 border border-white/10 backdrop-blur-xl shadow-2xl max-w-md mx-auto animate-[fadeUp_.8s_ease-out]">
        <h3 class="text-xl font-semibold text-white">Entrenamiento sugerido</h3>
        <p class="text-emerald-400 mt-2">Full Body · 45 min</p>

        <ul class="mt-4 space-y-2 text-gray-300">
          <li>🏋️ Sentadillas: 4x12</li>
          <li>🔥 HIIT: 12 min</li>
          <li>💪 Press banca: 4x10</li>
          <li>🧘 Estiramientos: 5 min</li>
        </ul>

        <button
          class="mt-6 w-full bg-emerald-400 text-black py-3 rounded-lg font-bold hover:bg-emerald-300 transition">
          Iniciar rutina
        </button>
      </div>
    </div>
  </section>

  <!-- FEATURES -->
  <section id="features" class="py-28 bg-gray-900">
    <div class="max-w-7xl mx-auto px-6 text-center">
      <h2 class="text-4xl font-extrabold text-white">Todo lo que necesitas para mejorar</h2>
      <p class="text-gray-300 mt-4 max-w-2xl mx-auto">
        Herramientas diseñadas para ayudarte a mantenerte constante, motivado y con progreso real.
      </p>

      <div class="grid md:grid-cols-3 gap-10 mt-16">
        <div class="p-6 bg-gray-800 rounded-xl border border-gray-700 hover:border-emerald-400 transition">
          <h3 class="text-2xl font-bold text-emerald-400">Planes inteligentes</h3>
          <p class="text-gray-300 mt-3">Rutinas generadas por IA basadas en tu rendimiento y objetivos.</p>
        </div>

        <div class="p-6 bg-gray-800 rounded-xl border border-gray-700 hover:border-emerald-400 transition">
          <h3 class="text-2xl font-bold text-emerald-400">Estadísticas avanzadas</h3>
          <p class="text-gray-300 mt-3">Métricas detalladas de fuerza, resistencia y progreso semanal.</p>
        </div>

        <div class="p-6 bg-gray-800 rounded-xl border border-gray-700 hover:border-emerald-400 transition">
          <h3 class="text-2xl font-bold text-emerald-400">Motivación constante</h3>
          <p class="text-gray-300 mt-3">Retos, logros y comunidad que te impulsa cada día.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- PROGRAMS -->
  <section id="programs" class="py-28 bg-gray-800">
    <div class="max-w-7xl mx-auto px-6">
      <h2 class="text-4xl font-extrabold text-white text-center">Programas profesionales</h2>

      <div class="grid md:grid-cols-3 gap-10 mt-16">
        <div class="bg-gray-900 p-6 rounded-xl border border-gray-700 hover:border-emerald-400 transition">
          <h3 class="text-xl font-bold text-white">Fuerza</h3>
          <p class="text-gray-300 mt-2">Gana músculo y mejora tu potencia.</p>
        </div>

        <div class="bg-gray-900 p-6 rounded-xl border border-gray-700 hover:border-emerald-400 transition">
          <h3 class="text-xl font-bold text-white">Resistencia</h3>
          <p class="text-gray-300 mt-2">Corre distancias más largas con menos esfuerzo.</p>
        </div>

        <div class="bg-gray-900 p-6 rounded-xl border border-gray-700 hover:border-emerald-400 transition">
          <h3 class="text-xl font-bold text-white">Pérdida de grasa</h3>
          <p class="text-gray-300 mt-2">Programas intensos para quemar grasa rápido.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- REVIEWS -->
  <section id="reviews" class="py-28 bg-gray-900">
    <div class="max-w-7xl mx-auto px-6">
      <h2 class="text-4xl font-extrabold text-white text-center">Lo que dicen nuestros atletas</h2>

      <div class="grid md:grid-cols-3 gap-10 mt-16">
        <div class="p-6 bg-gray-800 rounded-xl border border-gray-700">
          <p class="text-gray-300 italic">"Nunca había sido tan constante entrenando, Athletix me motivó como nunca."</p>
          <span class="block mt-4 text-emerald-400 font-bold">Andrea · Crossfit</span>
        </div>

        <div class="p-6 bg-gray-800 rounded-xl border border-gray-700">
          <p class="text-gray-300 italic">"Los reportes semanales me ayudaron a mejorar mi carrera a 5K."</p>
          <span class="block mt-4 text-emerald-400 font-bold">Luis · Runner</span>
        </div>

        <div class="p-6 bg-gray-800 rounded-xl border border-gray-700">
          <p class="text-gray-300 italic">"La IA recomienda entrenos brutales. Se siente como un entrenador real."</p>
          <span class="block mt-4 text-emerald-400 font-bold">Diego · Fitness</span>
        </div>
      </div>

    </div>
  </section>

  <!-- FOOTER -->
  <footer class="py-14 bg-black text-center text-gray-400">
    <h3 class="text-emerald-400 text-2xl font-bold">Athletix</h3>
    <p class="mt-2">Entrena más inteligente, no más duro.</p>
    <small class="block mt-4">© {{ year }} Athletix · Todos los derechos reservados</small>
  </footer>
</template>

<script setup lang="ts">
const year = new Date().getFullYear();
</script>

<style>
@keyframes fadeUp {
  from {
    opacity: 0;
    transform: translateY(40px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>
