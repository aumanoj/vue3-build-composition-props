<template>
  <div class="box">
    <span>Grand Child Component</span>
    <h1>{{ child_greeting }}</h1>
  </div>
</template>

<script setup>
  /* Defined props here */
  const props = defineProps({
    child_greeting: String,
    required: false
  })
</script>
  