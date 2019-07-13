<template>
  <div id="app">
      <SideNav />
      <profile :profile="profile"/>
      <Overview :overview="overview"/>
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
  },
  data() {
    return {
      profile: {
        followUps: [],
        details: {}
      },
      overview: {
        inventory: {},
        services: {},
        agreements: []
      }
      
    }
  },
  async created() {
    const profile = await fetch('http://localhost:3000/profile/1')
      .then(res => res.json())
    this.profile = profile

    const overviews = await fetch('http://localhost:3000/overview')
      .then(res => res.json())
      
    this.overview = overviews[0]
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Lato:300,400,700&display=swap');
  #app{
    display: flex;
    background-color: lightgrey;
    max-width: 100%;
    height: 100vh;
    border-radius: 10px;
    overflow: hidden;
    font-family: 'Lato', sans-serif;
  }



</style>
