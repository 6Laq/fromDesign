<template>
  <div class="main">
    <div class="row around-xs middle-xs m-bottom">
      <div class="col-xs-5">
        <span>Agreements</span>
        <span>03</span>
      </div>
      <div class="col-xs-5 end-xs">See All</div>
    </div>
    <div class="list row around-xs border-area small-bottom">
      <div class="col-xs-2 s-text small-bottom">Id</div>
      <div class="col-xs-4 s-text small-bottom">Price</div>
      <div class="col-xs-3 s-text small-bottom">Status</div>
      <div class="col-xs-3 s-text small-bottom">Cosignee</div>
    </div>
    <div class="list row around-xs">
      <div class="col-xs-2 s-text small-bottom id-number">#44545</div>
      <div class="col-xs-4 s-text small-bottom"><span>4500</span> <span>450 cf</span></div>
      <div class="col-xs-3 s-text small-bottom"><span class="id-number grey-box">Signed</span> <span>today</span></div>
      <div class="col-xs-3 s-text small-bottom">
        <i class="fas fa-arrow-right fa-xs "></i>
        <i class="fas fa-arrow-up fa-xs "></i>
        <i class="fas fa-ellipsis-h col-xs"></i>
      </div>
    </div>
    <div class="list row around-xs">
      <div class="col-xs-2 s-text small-bottom id-number">#88888</div>
      <div class="col-xs-4 s-text small-bottom"><span>3400</span> <span>490 cf</span></div>
      <div class="col-xs-3 s-text small-bottom"><span class="grey-box">canceled</span><span>Jan 12</span></div>
      <div class="col-xs-3 s-text small-bottom">
        <i class="fas fa-arrow-right fa-xs "></i>
        <i class="fas fa-arrow-up fa-xs "></i>
        <i class="fas fa-ellipsis-h col-xs"></i>
      </div>
    </div>
    <div class="list row around-xs">
      <div class="col-xs-2 s-text id-number">#01011</div>
      <div class="col-xs-4 s-text "><span>2500</span> <span>200 cf</span></div>
      <div class="col-xs-3 s-text "><span class="grey-box">canceled</span><span>Jan 12</span></div>
      <div class="col-xs-3 s-text ">
        <i class="fas fa-arrow-right fa-xs "></i>
        <i class="fas fa-ellipsis-h col-xs"></i>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  
}
</script>


<style scoped>
  .main{
    padding: 20px;
  }
  
  .s-text{
    font-size: .8em;
    color: grey;
  }

  .list{
    
  }

  .border-area{
    border-bottom: 1px solid lightgrey;
  }

  .m-bottom{
    margin-bottom: 30px;
  }

  .small-bottom{
    margin-bottom: 10px;
  }

  .id-number{
    color: blue
  }

  .grey-box{
    background-color: lightgray;
    border-radius: 3px;
  }
</style>