<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div class="min-h-screen flex flex-col bg-slate-100">
    <!-- Навбар -->
    <header class="sticky top-0 z-10 bg-white border-b border-slate-200 shadow-sm">
      <div class="max-w-4xl mx-auto flex items-center justify-between px-6 py-3">
        <div class="font-bold text-xl tracking-[0.04em]">
          MyApp
        </div>

        <nav class="flex gap-4">
          <RouterLink
            to="/"
            class="text-sm px-3 py-1.5 rounded-full transition
                   hover:bg-indigo-50 hover:-translate-y-px
                   text-slate-800"
          >
            Home
          </RouterLink>

          <RouterLink
            to="/about"
            class="text-sm px-3 py-1.5 rounded-full transition
                   hover:bg-indigo-50 hover:-translate-y-px
                   text-slate-800"
          >
            About
          </RouterLink>

          <RouterLink
            to="/contact"
            class="text-sm px-3 py-1.5 rounded-full transition
                   hover:bg-indigo-50 hover:-translate-y-px
                   text-slate-800"
          >
            Contact
          </RouterLink>
        </nav>
      </div>
    </header>

    <!-- Контент -->
    <main class="flex-1 max-w-4xl mx-auto w-full px-6 py-6">
      <RouterView />
    </main>

    <!-- Футер -->
    <footer class="bg-white border-t border-slate-200">
      <div class="max-w-4xl mx-auto px-6 py-3 text-center text-sm text-slate-600">
        <p>
          Звʼязатися зі мною:
          <a
            href="mailto:anastasiia.storozhuk@oa.edu.ua"
            class="text-indigo-600 hover:underline"
          >
            anastasiia.storozhuk@oa.edu.ua
          </a>
        </p>
      </div>
    </footer>
  </div>
</template>
