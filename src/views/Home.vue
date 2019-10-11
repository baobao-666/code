<template>
  <div class="home_page">
    <div class="home_header">头部</div>
    <Swiper></Swiper>
    <NavList :data='List' ></NavList>
  </div>
</template>

<script>
import Swiper from "@/components/Home/banner.vue";
import NavList from "@/components/Home/navList.vue";
export default {
  components: {
    Swiper,
    NavList
  },
  data(){
    return{
      List:[
        {
          title:'标签',
          img:'色块'
        },
        {
          title:'标签',
          img:'色块'
        },
        {
          title:'标签',
          img:'色块'
        },{
          title:'标签',
          img:'色块'
        },{
          title:'标签',
          img:'色块'
        }
      ]
    }
  }
};
</script>

<style  scoped>
.home_page {
  width: 100%;
  height: 100%;
  background: #666;
}
</style>