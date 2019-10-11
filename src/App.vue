<template>
  <div id="app">
<div class="app_main">
 <router-view/>
</div>
   <div class="app_footer">
     <router-link to="/home"  tag="span" >主页</router-link>
     <router-link to="/state" tag="span" >信息</router-link>
   </div>
  </div>
</template>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  list-style: none;
  box-sizing: border-box;
}
#app,html,body{
  width: 100%;
  height: 100%;
}
#app{
  display: flex;
  flex-direction: column;
}
.app_main{
  flex: 1;
}
.app_footer{
  width: 100%;
  line-height: 50px;
  display: flex;
  span{
    flex: 1;
    text-align: center;
    &.router-link-active{
      color: skyblue;
    }
  }
}
</style>
