<template>
  <div id="app">
    <Nav title="My App" v-bind:links="linkss" />
   title:{{titles}} <br>
   product:{{product}} <br>
   number:{{number}}

    <Footer v-bind:product="product" v-bind:title="titles"  />
  </div>
</template>

<script>
import Nav from './components/Nav.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Nav,Footer
  },
  data:function(){
      return {
        titles:'Product',
        product:'Book',
        number:0,
      linkss:[{
        name:'home',url:'/home'
      },{
        name:'Contact',url:'/contact'
      }]
      }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
}
</style>
