<template>
  <h1>App Component</h1>
  <!-- Count sample  -->
  <p>Count: {{ count }}</p>
  <button @click="count++">Increment Count</button>
  <!-- Included Parent component with props-->
  <GreetingParent :message="greetingMessage" />
</template>

<script setup>
import { ref } from 'vue';
import GreetingParent from './components/GreetingParent.vue';
  const count = ref(0);
  const greetingMessage = 'Greeting from App.vue';
</script>
