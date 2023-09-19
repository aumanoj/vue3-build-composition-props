<template>
  <h1>App Component</h1>
  <!-- Counter sample  -->
  <Counter/>
  <!-- Included Parent component with props-->
  <GreetingParent :message="greetingMessage" />
</template>

<script setup>
  import { ref } from 'vue'
  import Counter from './components/Counter.vue'
  import GreetingParent from './components/GreetingParent.vue'
  const greetingMessage = ref('Greeting from App.vue')
</script>
