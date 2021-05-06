<template> 
<div class="nav">
    <h3>
    <ul v-for="link in links" :key="link.name">
    <li><a v-bind:href="link.url">{{link.name}}</a></li>
    </ul>
    </h3>
</div>
</template>


<script>
export default {
  name: 'Nav',
  props: {
    title: String,
    links:Array
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {

}
.nav{
  height:50px;
  background:red;
  width:100%
}
</style>
