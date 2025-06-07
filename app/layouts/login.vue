<template>
  <div>
    <p>Login</p>
    <slot/> 
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const email = ref('')
const password = ref('')

function handleLogin() {
  // Simple mock action
  alert(`Logging in with\nEmail: ${email.value}\nPassword: ${password.value}`)
}
</script>

<style scoped>
/* Optional: add custom styling if needed */
</style>
