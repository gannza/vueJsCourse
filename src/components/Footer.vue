<template> 
<div class="nav">
    <h3>Footer</h3>
     title:{{til}} <br>
   product:{{prod}} <br>
   number:{{number}}
</div>
</template>

<script>
export default {
  name: 'Footer',
  props:{
     product:String,title:String
  },
    data:function(){
        return {
        til:this.title,
        prod:this.product,
        number:0
        }
  }
}
</script>