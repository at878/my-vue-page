<template>
  <main class="container">
    <h1 class="title">Hello, Vue 3 + Vite</h1>
    <p class="author">By 沈剑皓</p>
    <p class="subtitle">This is a fancy page crafted with ❤️ and composability.</p>
    <button @click="count++" class="btn">Click Me ({{ count }})</button>
  </main>
</template>

<script setup>
import { ref } from 'vue'
const count = ref(0)
</script>

<style scoped>
.container {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
  color: white;
  font-family: 'Segoe UI', sans-serif;
  text-align: center;
}

.title {
  font-size: 3rem;
  font-weight: bold;
  margin-bottom: 0.5rem;
  text-shadow: 1px 1px 4px rgba(0,0,0,0.3);
}

.author {
  font-size: 1.5rem;
  font-weight: 600;
  color: #ffd700;
  margin-bottom: 1rem;
  animation: pulse 2s infinite ease-in-out;
  text-shadow: 1px 1px 6px rgba(255, 255, 255, 0.4);
}

.subtitle {
  font-size: 1.2rem;
  margin-bottom: 2rem;
  opacity: 0.9;
}

.btn {
  padding: 0.75rem 1.5rem;
  background-color: #ffffff22;
  border: none;
  border-radius: 8px;
  color: white;
  font-size: 1rem;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.btn:hover {
  background-color: #ffffff44;
}

@keyframes pulse {
  0%, 100% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.07);
  }
}
</style>
