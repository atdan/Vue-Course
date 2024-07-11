<script setup>
import { ref } from 'vue'

const isTrue = true
const isFalse = false

let isVisible = ref(true)

let isUserLoggedIn = ref(false)
let username = 'Shanks'
let showDetails = ref(isUserLoggedIn)

const isActive = ref(false)

let password = ref(0)
</script>

<template>
  <div>
    <p v-if="isTrue">This will show if isTrue is true</p>
    <p v-else-if="isFalse">This will show if isFalse is true</p>
    <p v-else>This will show if neither isTrue or isFalse is true</p>
  </div>

  <p v-show="isVisible">This will be shown or hidden based on the value of isVisible</p>
  <button @click="isVisible = !isVisible">Toggle Visibility</button>

  <div>
    <h1 v-if="isUserLoggedIn">Welcome, {{ username }}</h1>
    <p v-else>Please log in to access this content</p>

    <h4 v-show="showDetails">You're now able to modify your dashboard</h4>
  </div>

  <div v-if="isActive">
    <h2>Content Header</h2>
    <p>
      Content Details, Lorem ipsum dolor sit amet consectetur adipisicing elit. Porro deleniti
      maxime autem eum iure doloribus voluptatibus aliquid, consequuntur voluptate eaque ratione
      necessitatibus veniam! Sit alias odit a! Odio, beatae quibusdam?
    </p>
  </div>

  <button @click="isActive = !isActive">Toggle Post</button>

  <div>
    <h1 v-if="password.length >= 8">Strong password</h1>
    <h1 v-else-if="password.length < 8">Weak password</h1>
    <h1 v-else>Enter Your password</h1>
  </div>
</template>
