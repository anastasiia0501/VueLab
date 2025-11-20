<script setup lang="ts">
defineProps<{
  username: string,
  isActive: boolean
}>()
</script>

<template>
  <!-- 
    Ми застосовуємо класи Tailwind.
    Умовна логіка :class тепер просто перемикає різні класи Tailwind!
  -->
  <div
    class="border p-4 mt-3 rounded-lg shadow-sm
          bg-white border-gray-300
          dark:bg-gray-800 dark:border-gray-600"
  >
    <h3 class="font-semibold text-lg dark:text-white">{{ username }}</h3>
    <p
      class="text-sm"
      :class="isActive
        ? 'text-green-700 dark:text-green-300'
        : 'text-gray-500 dark:text-gray-400'"
    >
      Статус: {{ isActive ? 'Онлайн' : 'Офлайн' }}
    </p>
  </div>
</template>