<template>
  <!-- <h1 :class="$style['m-class']">Using Module CSS with $ syntax (kabak-case)</h1> -->

  <h1 :class="moduleClasses.anotherClass">Using module CSS with $ syntax (camelCase)</h1>
</template>

<style module="moduleClasses">
/* kabab case */
.m-class {
  background: firebrick;
  color: white;
}

.anotherClass {
  background: seagreen;
  color: white;
}
</style>
