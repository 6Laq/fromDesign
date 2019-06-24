<template>
  <div class="profile">
    <div>

      <div class="profile-main">
        <div class="aboveName row">
          <div class="signed col-xs">
            <span class="signed-title ">
              Signed
            </span>
          </div>
          <i class="fas fa-folder col-xs-2"></i>
          <i class="fas fa-ellipsis-h col-xs-2"></i>
        </div>
        <div class="namedappt">
          <div class="name-plate m-bottom">
            <h2>Benny</h2>
            <h2>Bahamas</h2>
          </div>
          <div class="i-group m-bottom">
            <i class="fas fa-arrow-up fa-xs p-icon"></i>
            <i class="fas fa-arrow-up fa-xs p-icon"></i>
            <i class="fas fa-arrow-up fa-xs p-icon"></i>
          </div> 
          <div class="m-bottom">
            <div>2/5 follow ups</div>
            <progress value="2" max="5" class="progress-bar col-xs-11"></progress>
          </div>
          <div class="followups">
            <div class="followup row middle-xs" v-for="followup of followups" :key="followup.address" >
              <div class="col-xs-2 arrow">
                <i class="fas fa-arrow-up fa-xs "></i>
              </div>
              <div class="col-xs">
                <div class="date">{{followup.date}}</div>
                <div class="address tiny grey">{{followup.address}}</div>
              </div>
              <div class="col-xs-2">
                <i class="fas fa-chevron-right fa-xs"></i>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div>
      <div class="profile-bottom">
        <div class="details">
          <div class="details-title">
            <p>
              <i class="fas fa-align-left fa-xs"></i>
              Details
            </p>
          </div>
          <div class="under-details">
            <div class="row between-xs m-bottom">
              <div class="col-xs-4 s-text">company</div>
              <div class="col-xs-8 s-text">East coast movers</div>
            </div>
            <div class="row m-bottom between-xs">
              <div class="col-xs-4 s-text">Assigned To</div>
              <div class="col-xs-8 s-text">Alex Just</div>
            </div>
          </div>
        </div>
        <div class="appointment ">
          <div class="appointments row between-xs middle-xs">
            <div class="col-xs-1 arrow">
              <i class="fas fa-arrow-up fa-xs "></i>
            </div>
            <div class="col-xs ">
              <div class="appointment-type tiny grey">Next Appointment</div>
              <div class="appointment-addy"><small>Today at 3pm</small></div>
            </div>
            <div class="col-xs-1">
              <i class="fas fa-chevron-right fa-xs"></i>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

</template>

<script>


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
.s-text {
  font-size: .8em;
}
.m-bottom {
  margin-bottom: 20px;
}
.p-icon {
  padding: 0px 10px;
}
.aboveName {
  margin-bottom: 50px;
}

.name-plate {
  margin-bottom: 20px;
}

.name-plate h2 {
  margin: 0px;
}

.signed-title {
  background: lightblue;
  color: blue;
  font-size: .8em;
  padding: 3px;
  border-radius: 3px;
}

.profile {
  background: white;
  padding: 40px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

  .progress-bar{
    width: 225px;
  }


  .assignee, .company-name{
    text-align: right;
  }

  .details-title{
    border-bottom: solid 1px lightgrey;
    text-align: left;
  }

  .followup {
    border-bottom: 1px solid rgba(0,0,0, 0.2);
    padding: 10px 0px;
  }

  .tiny {
    font-size: .6em;
  }
  .grey {
    color: grey;
  }

  .date {
    font-size: .8em;
    font-weight: bold;
  }

  .details {
    margin-bottom: 50px;
  }

  .appointments {
    padding: 10px;
    border-radius: 3px;
    background: lightgreen;

  }
</style>
