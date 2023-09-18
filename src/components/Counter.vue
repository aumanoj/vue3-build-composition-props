<template>
  <p>Count: {{ count }}</p>
  <label for="increment">Increment Value:</label>
  <input type="number" id="increment" v-model="incrementValue" />
  <button @click="incrementCounter(incrementValue)">Increment</button>
</template>
<script setup>
  import {ref} from 'vue'
  const count = ref(0)
  const incrementValue = ref(1)
  const incrementCounter = (value)  =>{
    count.value += parseInt(value)
  }
</script>
<style scoped>
label{
    padding: 15px;
}
button{
    margin-left: 10px;
}
input {
  width: 70px;
  margin: 10 auto;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
}
</style>