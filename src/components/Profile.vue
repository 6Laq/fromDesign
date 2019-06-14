<template>
  <div class="profile-main">
    <div class="aboveName">
      <span class="signed">Signed</span>
      <i class="fas fa-folder"></i>
      <i class="fas fa-ellipsis-h"></i>
    </div>
    <div class="namedappt">
      <span class="name-plate">
        <h2>Benny Bahamas</h2>
      </span>
      <p>2/5 follow ups</p>
      <div class="dates">
        <div class="date-set">
          <span><i class="fas fa-arrow-up fa-xs "></i></span>
          <small><b>03/03/88</b></small>
          <small>address address address</small>
          <i class="fas fa-chevron-right fa-xs"></i>
        </div>
      </div>
    </div>
    <div class="details">
      <div class="details-title">
        <i class="fas fa-align-left fa-xs"></i>
        <h5>Details</h5>
      </div>
      <div>
        <h5>Company</h5>
      </div>
    </div>
    <div class="appointment">
      <small>next appointment</small>
      <small><b>TODAY 3PM</b></small>
      <i class="fas fa-arrow-right fa-xs"></i>
    </div>
  </div>
</template>

<script>
import 'flexboxgrid';

export default {
  
}
</script>


<style scoped>
  .profile-main{
    display: flex;
    flex-direction: column;
    justify-content: center;
    height: 700px;
    width: 300px;
    margin: 0px 0px 0px 0px;
    padding: 0px 10px 0px 0px;
    background-color: white;
    border-left: solid 1px lightgray;
  }

  .aboveName{
    margin: 0px 0px 10px 20px;
    align-content: space-between;
  }

  .signed{
    background-color: lightgray;
    color: darkcyan;
  }

  hr{
    width: 250px;
  }

  .namedappt{
    height: 300px;
    width: 250px;
    margin: 0px 0px 0px 20px;
  }

  .name-plate{
    flex-direction: column;
  }

  .appointment{
    width: 250px;
    height: 50px;
    margin: 15px 0px 0px 20px;
    background-color: lightseagreen;
    border-radius: 5px;
  }

  .details{
    margin: 50px 0px 10px 30px;
    
  }

  .details-title{
    border-bottom: solid 1px lightgrey;
    flex-direction: row;
  }


  .date-set{
    width: 250px;
    height: 50px;
    background-color: aquamarine;
    flex-direction: column;
  }
</style>
