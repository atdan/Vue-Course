<script setup>
import { reactive } from 'vue'

let initialState = reactive({ val: { count: 0 }, user: ['Daniel', 'James'] })

const changeUser = () => {
  initialState.user[0] = 'Clark'
  initialState.user[1] = 'Bruce'
}
</script>

<template>
  <h1>Count: {{ initialState.count }}</h1>
  <h2>Users: {{ initialState.user }}</h2>

  <button @click="initialState.val.count++">+</button>
  <button @click="initialState.val.count--">-</button>
  <button @click="changeUser">Change User</button>
  <button @click="initialState.user.push('Wayne')">Add new User</button>
</template>
