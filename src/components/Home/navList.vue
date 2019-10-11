<template>
  <div class="nav-page">
      <div class="nav-wrap" v-for="(item,index) in data"  :key="index">
       <div class="nav-title"> {{item.title}}</div> 
       <div class="nav-logo"></div>
        </div>
  </div>
</template>

<script>
export default {
props:{
  data:{
    type:Array,
    default(){
      return [
        {
          title:'空',
          img:'空'
        }
      ]
    }
  }
}
}
</script>

<style scoped >
.nav-page{
  width: 100%;
height: 200px;
}
 .nav-wrap{
   width: 100%;
   
 }
</style>