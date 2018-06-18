<template>
  <div id="app">
    <hist-navbar></hist-navbar>
    <router-view/>
  </div>
</template>

<script>

import Navbar from './components/shared/Navbar'
/*import Vue from 'vue'

var example1 = new Vue({
  el: '#histNavbar',

  methods: {
    itemMenuClicked: function itemMenuClicked (title) {
      $('.nav-item > a').removeClass('colored-green-border')
      $(title).addClass('colored-green-border')
    }
  }
})*/

export default {
  components: {
    'hist-navbar': Navbar
  },
  name: 'App'
}

</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>
