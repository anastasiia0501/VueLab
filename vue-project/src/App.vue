<script setup lang="ts"></script>

<template>
  <div class="app">
    <header class="navbar">
      <div class="logo">MyApp</div>

      <nav class="nav-links">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/contact">Contact</RouterLink>
      </nav>
    </header>

    <main class="main-content">
      <RouterView />
    </main>

    <footer class="footer">
      <p>
        Звʼязатися зі мною:
        <a href="mailto:anastasiia.storozhuk@oa.edu.ua">anastasiia.storozhuk@oa.edu.ua</a>
      </p>
    </footer>
  </div>
</template>

<style scoped>
.app {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  background: #f5f5f7;
}

.navbar {
  position: sticky;
  top: 0;
  z-index: 10;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 12px 24px;
  background: #ffffff;
  border-bottom: 1px solid #e2e2e2;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.04);
}

.logo {
  font-weight: 700;
  font-size: 20px;
  letter-spacing: 0.04em;
}

.nav-links {
  display: flex;
  gap: 16px;
}

.nav-links a {
  text-decoration: none;
  font-size: 14px;
  padding: 6px 12px;
  border-radius: 999px;
  transition: background 0.2s ease, color 0.2s ease, transform 0.1s ease;
  color: #333;
}

.nav-links a:hover {
  background: #f0f0ff;
  transform: translateY(-1px);
}

.nav-links .router-link-active {
  background: #4f46e5;
  color: #ffffff;
}

/* Контент розтягується, щоб футер був внизу */
.main-content {
  flex: 1;
  padding: 24px;
}

/* Футер */
.footer {
  padding: 12px 24px;
  text-align: center;
  font-size: 14px;
  color: #555;
  background: #ffffff;
  border-top: 1px solid #e2e2e2;
}

.footer a {
  color: #4f46e5;
  text-decoration: none;
}

.footer a:hover {
  text-decoration: underline;
}
</style>
