<template>
  <div class="container">
    <div class="row nav">
      <h2>Overview</h2>
      <h2>Services</h2>
      <h2>Contract</h2>
      <i class="fas fa-address-book fa-lg"></i>
    </div>
    <div class="row content">
      <div class="booking">
        
        <booking />
      </div>
      <div class="inventory"> 
        <Inventory />
      </div>
      <div class="services">
        
        <Services />
      </div>
      <div class="agreements">
        
        <agreements />
      </div>
    </div>
  </div>
</template>

<script>
import Inventory from './Inventory'
import Services from './Services'
import Agreements from './Agreements'
import Booking from './Booking'
import 'flexboxgrid';

export default {
  
  components: {
    Inventory,
    Services,
    Agreements,
    Booking
  }
}
</script>


<style scoped>
  .container{
    width: 700px;
    height: 700px;
    padding: 10px 30px 0px 30px;
    background-color:lightgray;
    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;
  }

  .content{
    justify-content: center;
    margin: 30px 0px 0px 0px;
  }

  .booking{
    width: 540px;
    height: 100px;
    background-color: white;
    margin: 10px;
    padding: 10px;
    border-radius: 10px;
  }

  .inventory{
    width: 250px;
    height: 175px;
    background-color: white;
    margin: 10px;
    padding: 10px;
    border-radius: 10px;
  }

  .services{
    width: 250px;
    height: 175px;
    background-color: white;
    margin: 10px;
    padding: 10px;
    border-radius: 10px;
  }

  .agreements{
    width: 540px;
    height: 175px;
    background-color: white;
    margin: 10px;
    padding: 10px;
    border-radius: 10px;
  }

  .nav{
    justify-content: space-around;
    border-bottom: solid 1px blue;
  }

  i{
    padding: 10px;
    margin: 15px 0px 0px 0px;
  }
</style>