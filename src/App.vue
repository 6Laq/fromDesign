<template>
  <div id="app">
    
      <SideNav class="sidenav " />
      <profile class="profile " />
    
  
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
  #app{
    display: flex;
    background-color: lightgrey;
    max-width: 100%;
    height: 700px;
    border-radius: 10px;
    overflow: hidden;
  }

</style>
