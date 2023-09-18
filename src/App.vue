<template>
  <h1>App Component</h1>
  <!-- Counter sample  -->
  <Counter/>
  <!-- Included Parent component with props-->
  <GreetingParent :message="greetingMessage" />
</template>

<script setup>
  import Counter from './components/Counter.vue'
  import GreetingParent from './components/GreetingParent.vue'
  const greetingMessage = 'Greeting from App.vue'
</script>
