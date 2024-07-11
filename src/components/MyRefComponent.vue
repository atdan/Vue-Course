<script setup>
import { ref } from 'vue'

let count = ref(0)

let username = ref('')

let usersList = ref(['Luffy', 'Mihawk', 'Shanks', 'Zoro', 'Jinbe'])

let userInfo = ref({ name: 'Alex', age: 21, location: ['ABJ', 'IDK'], isMarried: false })
</script>

<template>
  <h1>Count: {{ count }}</h1>

  <button @click="count++">+</button>
  <button @click="count--">-</button>

  <h1>Username: {{ username }}</h1>
  <button @click="username = 'Jordan'">Add User</button>

  <h1>Users List: {{ usersList }}</h1>
  <button @click="usersList.push('Ace')">Add User</button>

  <h1>Name: {{ userInfo.name }}</h1>
  <h1>Age: {{ userInfo.age }}</h1>
  <h1>Location: {{ userInfo.location }}</h1>
  <h1>IsMarried: {{ userInfo.isMarried }}</h1>

  <button @click="userInfo.name = 'Sam'">Change Name</button>
  <button @click="userInfo.age = 40">Change Age</button>
  <button @click="userInfo.location = ['LAG', 'DUB']">Change Location</button>
  <button @click="userInfo.isMarried = true">Change Marital status</button>
</template>
