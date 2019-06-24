<template>
  <div id="app">
    
      <SideNav class="sidenav " />
      <profile />
    
  
      <Overview class="overview " />
    
  </div>
</template>

<script>
import Profile from './components/Profile.vue'
import Overview from './components/Overview'
import SideNav from './components/SideNav'
import 'flexboxgrid'

export default {
  components: {
    Profile,
    Overview,
    SideNav
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Lato:300,400,700&display=swap');
  #app{
    display: flex;
    background-color: lightgrey;
    max-width: 100%;
    height: 700px;
    border-radius: 10px;
    overflow: hidden;
    font-family: 'Lato', sans-serif;
  }


</style>
