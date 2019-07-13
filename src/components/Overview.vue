<template>
  <div class="container">
    <div class="inner-content">
      <div class="row between-xs middle-xs tabs">
        <div class="col-xs-8 around-xs">
          <div class="row">
            <div class="col-xs">
              <span>Overview</span>
            </div>
            <div class="col-xs">
              <span>Inventory</span>
            </div>
            <div class="col-xs">
              <span>Services</span>
            </div>
            <div class="col-xs">
              <span>Contract</span>
            </div>
          </div>
        </div>
          
        <div class="col-xs right-text">
          <i class="fas fa-address-book fa-lg"></i>
        </div>
      </div>
      <div class="row around-xs content">
        <div class="col-xs-11 booking m-bottom">
          <booking />
        </div>
        <div class="col-xs-5 inventory m-bottom"> 
          <Inventory :inventory="overview.inventory"/>
        </div>
        <div class="col-xs-5 services m-bottom">
          <Services :services="overview.services"/>
        </div>
        <div class="col-xs-11 agreements">
          <agreements :agreements="overview.agreenments"/>
        </div>
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
  props: {
    overview: {}
  },
  
  components: {
    Inventory,
    Services,
    Agreements,
    Booking
  }
}
</script>


<style scoped>
  .m-bottom{
    margin-bottom: 30px;
  }

  .tabs{
    margin: 0px auto;
  }

  .inner-content{
    margin: 0px auto;
    max-width: 1200px;
  }

  .container{
    padding: 10px 30px;
    background-color: rgba(250,250,250, .8);
  }

  .content{
    margin: 30px 0px;
  }

  .booking{
    width: 540px;
    background-color: white;
    padding: 10px;
    border-radius: 10px;
  }

  .inventory{
    width: 250px;
    background-color: white;
    padding: 10px;
    border-radius: 10px;
  }

  .services{
    width: 250px;
    background-color: white;
    padding: 10px;
    border-radius: 10px;
  }

  .agreements{
    width: 540px;
    background-color: white;

    padding: 10px;
    border-radius: 10px;
  }

  .nav{
    border-bottom: solid 1px blue;
    font-size: 1.2em;
  }

  i{
    padding: 10px;
    margin: 15px 0px 0px 0px;
  }
  .right-text {
    text-align: right;
  }
</style>