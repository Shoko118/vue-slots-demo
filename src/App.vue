<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <Welcome>
    <template #demo>
      <h1>template name</h1>
    </template>
    <template #firstName="{ middleName, lastName }">
      <h1>Slot firstName of middel name {{ middleName }}</h1>
      <h1>Slot firstName of last name {{ lastName }}</h1>
    </template>
  </Welcome>
</template>

<script setup>
import Welcome from "./components/Welcome.vue";
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
