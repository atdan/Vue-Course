<!-- JS -->
<script setup>
// const myMessage = 'Hello Component'
// const myNumber = 100

// function add(x, y) {
//   return x + y
// }

const myGithub = 'https://github.com/atdan?tab=repositories'
// const onePieceImage =
//   'http://www.pixelstalk.net/wp-content/uploads/2016/03/One-piece-picture-HD.jpg'
// const altText = 'Just a random image'

// const imageWidth = 400
// const imageHeight = 400

// Dynamic Binding -----------
// eslint-disable-next-line no-unused-vars
const imageInfo = {
  src: 'http://www.pixelstalk.net/wp-content/uploads/2016/03/One-piece-picture-HD.jpg',
  alt: 'Just a random image',
  width: 400,
  height: 400
}
</script>

<!-- HTML -->
<template>
  <!-- <h1>{{ myMessage }}</h1>
  <h2>{{ myNumber }}</h2>
  <h3>2 + 2 = {{ add(2, 2) }}</h3> -->

  <!-- <a v-bind:href="myGithub">My Github</a> -->
  <a :href="myGithub">My Github</a>

  <!-- <img :src="onePieceImage" :alt="altText" :width="imageWidth" :height="imageHeight" /> -->

  <img :="imageInfo" />
</template>

<!-- CSS -->
<style>
h1 {
  color: red;
}
</style>
