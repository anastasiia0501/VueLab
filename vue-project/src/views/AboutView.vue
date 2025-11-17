<script setup lang="ts">
const techs = ['Vue 3', 'TypeScript', 'Vue Router']
</script>

<template>
  <div class="about">
    <h1>Про цей проєкт</h1>

    <p class="lead">
      Це проста тестова програма на Vue, де я тренуюсь з роутінгом,
      компонентами та стилями.
    </p>

    <h2>Стек технологій</h2>
    <ul class="tech-list">
      <li v-for="tech in techs" :key="tech">
        {{ tech }}
      </li>
    </ul>

    <p class="note">
      Можна додати ще сторінки, форму контакту, авторизацію тощо — це вже поле
      для експериментів 🙂
    </p>
  </div>
</template>

<style scoped>
.about {
  padding: 24px;
}

.lead {
  margin: 12px 0 20px;
  color: #555;
  max-width: 600px;
}

.tech-list {
  list-style: none;
  padding: 0;
  margin-bottom: 20px;
}

.tech-list li {
  padding: 6px 10px;
  border-radius: 999px;
  border: 1px solid #e5e5e5;
  display: inline-block;
  margin-right: 8px;
  margin-bottom: 8px;
  font-size: 14px;
}

.note {
  font-size: 14px;
  color: #777;
  max-width: 600px;
}
</style>
