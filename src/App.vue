
<template>
  <div class="counter">
    <h1>شمارنده من</h1>

    <h2>{{ count }}</h2>

    <div class="buttons">
      <button @click="count++">افزایش +</button>

      <button @click="count--">کاهش -</button>

      <button @click="count = 0">ریست</button>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const count = ref(0)
</script>

<style scoped>
.counter {
  text-align: center;
  margin-top: 100px;
  font-family: Arial, sans-serif;
}

h1 {
  color: #333;
}

h2 {
  font-size: 50px;
  color: #472D1F;
  margin: 20px;
}

.buttons {
  display: flex;
  justify-content: center;
  gap: 10px;
}

button {
  padding: 12px 20px;
  border: none;
  border-radius: 8px;
  background-color: #472D1F;
  color: white;
  cursor: pointer;
  font-size: 16px;
}

button:hover {
  background-color: #472D1F;
}
</style>
