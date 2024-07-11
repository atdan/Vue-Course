<script setup>
import { computed, ref } from 'vue'

// const number = ref(5)
// const squaredNumber = computed(() => {
//   return number.value * number.value
// })

// const firstName = ref('hancock')
// const lastName = ref('Boa')

// const fullName = computed(() => {
//   return firstName.value + ' ' + lastName.value
// })

const counter = ref(0)
const squaredCounter = computed(() => counter.value ** 2)
const incrementCounter = () => counter.value++
</script>

<template>
  <!-- <h1>Original Number: {{ number }}</h1>
  <h1>Squared Number: {{ squaredNumber }}</h1>

  <h1>Fullname: {{ fullName }}</h1> -->

  <h1>Counter: {{ counter }}</h1>
  <h1>Squared Counter: {{ squaredCounter }}</h1>
  <button @click="incrementCounter">Increment Counter</button>
</template>
