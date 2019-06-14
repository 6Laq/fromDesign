<template>
  <div class="sidenav">
    <div class="top-icons">
      <i class="fas fa-arrow-alt-circle-down fa-lg"></i>
      <i class="fas fa-arrow-alt-circle-up fa-lg active"></i>
      <i class="fas fa-arrow-alt-circle-down fa-lg"></i>
      <i class="fas fa-arrow-alt-circle-up fa-lg"></i>
      <i class="fas fa-arrow-alt-circle-down fa-lg"></i>
      <i class="fas fa-arrow-alt-circle-up fa-lg"></i>
    </div>
    <div class="lower-icons">
      <i class="fas fa-burn fa-2x"></i>
      <i class="fas fa-user fa-2x"></i>
    </div>
  </div>
</template>

<script>
import 'flexboxgrid'

export default {
  
}
</script>


<style scoped>
  .sidenav{
    background-color: white;
    height: 790px;
    width: 50px;
    max-width: 50px;
    padding: 5px;
    border-top-left-radius: 10px;
    border-bottom-left-radius: 10px;
  }

  .top-icons, .lower-icons{
    padding: 10px;
  }

  .active{
    color: cadetblue;
    border-left: solid 1px cadetblue;
  }

  i{
    margin: 20px 0px 0px 0px;
    color: lightgray;
  }

  .lower-icons{
    margin-top: 275px;
  }
</style>