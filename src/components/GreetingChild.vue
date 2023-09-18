<template>
  <div class="box">
  <span>Child Component</span>
  <h1>{{ parent_greeting }}</h1>
  <!-- Grand child component -->
  <GreetingGrandChild :child_greeting="parent_greeting"></GreetingGrandChild>
</div>
</template>
<script setup>
  import GreetingGrandChild from './GreetingGrandChild.vue'
  /* Defined props here */
  const props = defineProps({
    parent_greeting: String,
  })
</script>
  