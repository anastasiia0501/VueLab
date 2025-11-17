<script setup lang="ts">
const title = 'Головна сторінка'
const subtitle = 'Ласкаво просимо до мого маленького Vue-проєкту 👋'
</script>

<template>
  <div class="home">
    <h1>{{ title }}</h1>
    <p class="subtitle">
      {{ subtitle }}
    </p>

    <section class="cards">
      <div class="card">
        <h2>Що це?</h2>
        <p>Проста демо-сторінка, щоб потренуватись з Vue Router.</p>
      </div>

      <div class="card">
        <h2>Куди далі?</h2>
        <p>Перейди в меню та відкрий сторінку “About” або “Contact”.</p>
      </div>
    </section>
  </div>
</template>

<style scoped>
.home {
  padding: 24px;
}

.subtitle {
  margin-top: 8px;
  margin-bottom: 24px;
  color: #555;
}

.cards {
  display: grid;
  gap: 16px;
}

.card {
  padding: 16px;
  border-radius: 12px;
  background: #ffffff;
  border: 1px solid #e5e5e5;
  box-shadow: 0 1px 4px rgba(0, 0, 0, 0.03);
}
</style>
