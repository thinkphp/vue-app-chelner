<template lang="pug">

p {{ greeting }} to the App Chelner!

otherComponent

<div>
  <h2>Count: {{ counter }}</h2>
  <button @click="increaseClick()">Plus</button>
  <button @click="decreaseClick()">Minus</button>
</div>


<p class='footer'>Created by <a href='http://adrianstatescu.ch'>Adrian Statescu</a> using yarn create @vitejs/app app</p>

</template>

<script>

import otherComponent from './otherComponent.vue'

export default {

  components: {
  
   otherComponent
  
  },

  data() {
    return {
      greeting: 'Welcome ',
      counter: 0
    }
  },
  
  methods: {
  
    increaseClick () {
          
        this.counter = this.counter + 1 
    },
         
    decreaseClick () {
         
       this.counter = this.counter - 1  
         
    },
         
  }
}
</script>

<style lang="stylus">
p
  font-size 2em
  text-align center  
  font-family: verdana
p.footer
  font-size 1em
  text-align left
  font-family: verdana
  
</style>

