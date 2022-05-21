
<template>
  <div class="min-h-screen overflow flex flex-col justify-between">
    <div>
      <TopNav />
      <NavBar/>
      <Menu />
    </div>
    <div class="h-[380px] overflow-y-scroll px-24">
      <div class="grid grid-cols-4 gap-10 max-h-3/4 overflow-hidden mt-2">
        <div v-for="(card, i) in cards" :key="i" >
          <div class="text-[13px]">
            <Photo :src="`${card.src}`" class="w-full h-full " />
            <div class="py-1">
              <div class="text-gray-800 font-medium ">{{ card.title }}, {{ card.location }}</div>
              <div class="text-gray-500 ">{{ card.Artist }}</div>
              <div class="text-gray-500 ">{{ card.Date }}</div>
              <div class="text-gray-800 font-medium">$11,094 
                <span class="font-light text-gray-500">night</span>
              </div>
            </div>
          </div>
        </div>
      </div>
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
import Photo from './components/Photo.vue'

export default {
  name: 'App',
  components: {
    Menu,
    Foot,
    NavBar,
    TopNav,
    Photo
  },
  data() {
    return {
      cards: [
        {
          src: 'cards/5.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'cards/6.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'cards/7.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'cards/8.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'cards/9.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'cards/10.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
        {
          src: 'menuBar/Design.jpg',
          title: 'Gardone Riviera',
          location: 'Italy',
          Artist: 'Designed by David Chipperfield',
          Date: 'July 12-19'
        },
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: 'Poppins', sans-serif;
}
</style>
