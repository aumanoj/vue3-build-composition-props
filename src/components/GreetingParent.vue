<template>
  <div class="box">
  <span>Parent Component</span>
  <h1>{{ message }}</h1>
  <!-- Included Child Component -->
  <GreetingChild :parent_greeting="message" />
</div>
</template> 
<script setup>
import GreetingChild from './GreetingChild.vue';
/* Defined props here */
const props = defineProps({
  message: String,
})
</script>
  