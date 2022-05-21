
<template>
  <div class="min-h-screen overflow flex flex-col justify-between">
    <div>
      <TopNav />
      <NavBar/>
      <Menu />
      <!-- <div v-for="(menu,i) in menubar" :key="i">
        <div class="flex "> -->
          <!-- <Menu :src="`${menu.src}`" /> -->
        <!-- </div> -->
      <!-- </div> -->
    </div>
    <div class="overflow-hidden">
      
    </div>
    <div>
      <Foot />
    </div>
  </div>
</template>

<script>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import HelloWorld from './components/HelloWorld.vue'
import TopNav from './components/TaskBar.vue'
import NavBar from './components/NavBar.vue'
import Menu from './components/Menu.vue'
import Foot from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Menu,
    Foot,
    NavBar,
    TopNav
  },
}
</script>

<style>
#app {
  font-family: 'Poppins', sans-serif;
}
</style>
