<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import HelloWorld from './components/HelloWorld.vue'
import TopNav from './components/TaskBar.vue'
import NavBar from './components/NavBar.vue'
import Menu from './components/Menu.vue'
</script>

<template>
  <div class="max-h-screen overflow-hidden">
    <TopNav />
    <NavBar/>
    <Menu />
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Hello Vue 3 + Vite" />
  </div>
</template>

<style>
#app {
  font-family: 'Poppins', sans-serif;
}
</style>
