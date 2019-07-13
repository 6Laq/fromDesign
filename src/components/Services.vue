<template>
  <div class="serve">
    <div class="row around-xs middle-xs">
      <div class=" col-xs-1"><i class="circle-up fas fa-circle fa-xs"></i></div>
      <div class="col-xs-6"><h4>Services</h4></div>
      <div class="col-xs-2 end-xs"><i class="fas fa-arrow-right fa-xs "></i></div>
      
    </div>
    <div class="row around-xs">
      <div class="col-xs-7"><h2>{{services.cost}}</h2></div>
      <div class="col-xs-7">
        <div class=" border-area"><p>{{services.moreService}}</p></div>
        <div class=" ">
          <p>Insurance</p>
          <i class="fas fa-arrow-right fa-xs lower-icon"></i>
        </div>
      </div>
      
    </div>
  </div>
</template>

<script>
export default {
  props: {
    services: {
      type: Object,
      default() {
        return {}
      }
    }
  }
}
</script>


<style scoped>
  .circle-up {
    color: orange;
  }

  .border-area{
    border-bottom: 1px solid lightgrey
  }

  .lower-icon{
    
  }

</style>