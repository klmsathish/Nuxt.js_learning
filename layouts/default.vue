<template>
  <div>

    <Header @sidenavToggle ="displaySidenav = !displaySidenav"/>
    <SideNav 
     :show = "displaySidenav"
     @close = "displaySidenav = false"/>
     <Nuxt />
  </div>

</template>

<style>
html {
  font-family:'Open Sans', 'sans-serif';
}
body{
  margin:0; 
}
</style>
<script>
import Header from '@/components/navigation/TheHeader'
import SideNav from '@/components/navigation/TheSideNav'

export default {
  components:{
    Header,
    SideNav
  },
  data(){
    return{
      displaySidenav:false
    }
  }
}
</script>
