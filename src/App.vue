<script setup lang="ts">
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import Navbar from './components/Navbar.vue'
import Home from './components/Home.vue'
</script>

<template>
    <div id="app" class="w-screen h-screen font-Montserrat">
        <Home :nightMode=false />
    </div>
    <!-- <Person /> -->
  <!-- <header>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />
    </div>
  </header> -->

  <!-- <main>
    <TheWelcome />
  </main> -->
</template>

<style>
/* #app {
  font-family: "Montserrat", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
} */

.pgray {
  color: #535a5e;
}

.pblue {
  color: #669db3ff;
}
</style>
