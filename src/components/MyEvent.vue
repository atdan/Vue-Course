<script setup>
// import { ref } from 'vue'

// let counter = ref(0)
// const incrementCounter = () => counter.value++
// const decrementCounter = () => counter.value--

// const submitHandler = (e) => {
//   e.preventDefault()
//   alert('Valid credentials')
// }

const showMessage = (message) => alert(message)
</script>

<template>
  <!-- <h1>Count: {{ counter }}</h1>
  <button v-on:click="incrementCounter">Increment</button>
  <button @:click="decrementCounter">Decrement</button> -->

  <!-- <form @:submit="submitHandler">
    <input type="text" placeholder="Please enter your name" />
    <input type="email" placeholder="Please enter your email" />
    <button type="submit">Submit</button>
  </form> -->

  <button @click="showMessage('this is the message')">Show Message</button>
</template>
