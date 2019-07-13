<template>
  <div class="inven">
    <div class="row around-xs middle-xs">
      <div class=" col-xs-1"><i class="circle-up fas fa-circle fa-xs"></i></div>
      <div class="col-xs-6"><h4>Inventory</h4></div>
      <div class="col-xs-2 end-xs"><i class="fas fa-arrow-right fa-xs "></i></div>
      
    </div>
    <div class="row around-xs ">
      <div class="col-xs-7"><h2>{{inventory.cost}}</h2></div>
      <div class="col-xs-7">
        <div class=" border-area"><p>{{inventory.items}}</p></div>
        <div class=""><p>{{inventory.space}}</p></div>
      </div>
      
    </div>
  </div>
</template>

<script>
export default {
  props: {
    inventory: {
      type: Object,
      default() {
        return {}
      }
    }
  },
  data(){
    return {

    }
  }
}
</script>


<style scoped>
  .circle-up {
    color: royalblue;
  }

  .border-area{
    border-bottom: 1px solid lightgrey;
  }
</style>