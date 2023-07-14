<script setup>
    const message = 'Hello I am nazmul hossain. Today i am practiceing Vuejs.'
    const date = "<strong>10th July, 2023</strong>"
    const number = 11

    function getDate() {
      return "11th July, 2024"
    }

    function evenOrOdd(n) {
        if (n % 2 == 0) {
            return "Even"
        }
        return "Odd"
    }
</script>

<template>
  <div class="container mx-auto flex items-center justify-center min-h-screen flex-col">
       <h1 class="text-4xl">{{ message }}</h1>
       <h2 class="mt-10 text-xl text-gray-700">practiceing date is: {{ getDate() }}</h2>
       <!-- <h2>{{ number }} is {{evenOrOdd(number)}}</h2> -->
       <h2 class="mt-10 text-xl text-gray-700">{{ number }} is {{ number % 2 == 0 ? "Even" : "Odd" }}</h2>
  </div>
</template>

<style scoped>
  
</style>
