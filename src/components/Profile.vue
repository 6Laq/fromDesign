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
      <!-- <div class="dates">
        <div class="date-set">
          <p><i class="fas fa-arrow-up fa-xs "></i></p>
          <p><b>03/03/88</b></p>
          <p>address address address</p>
          <p><i class="fas fa-chevron-right fa-xs"></i></p>
        </div>
      </div> -->
      <div class="followups">
        <div class="followup row middle-xs" v-for="followup of followups" :key="followup.address" >
          <div class="col-xs-2">
            icon
          </div>
          <div class="col-xs">
            <div class="date">{{followup.date}}</div>
            <div class="address">{{followup.address}}</div>
          </div>
          <div class="col-xs-2">
            icon
          </div>
        </div>
      </div>
    </div>
    <div class="details">
      <div class="details-title">
        <p>
          <i class="fas fa-align-left fa-xs"></i>
          Details
        </p>
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
  data() {
    return {
      followups: [
        {date: '03/06/18', address: '1212 elm st, New York, Ny 12323'},
        {date: '03/06/18', address: '1232 tokyo ave, LA, CA 91021'}
      ]
    }
  }
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
    text-align: left;
  }


  .date-set{
    width: 250px;
    height: 75px;
    font-size: 15px;
    background-color: aquamarine;
    text-align: center;
  }
  .followup {
    border-bottom: 1px solid rgba(0,0,0, 0.2);
    padding: 10px 0px;
  }

  .address {
    font-size: .8em;
    color: grey;
  }

  .date {
    font-size: 1em;
    font-weight: bold;
  }
</style>
