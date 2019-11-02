<template>
   <div id="content">
    <!--  <div class="left">
          <div class="container-flex">
              <div class="row">
                  <div class="col-md-12">
                      <app-nav></app-nav>
                  </div>
              </div>
          </div>
      </div>
      <div class="right">
          <div class="container-flex app-header">
              <div class="row">
                  <div class="col-md-12">
                      <app-header></app-header>
                  </div>
              </div>
          </div>
          <div class="container-flex app-cards">
              <div class="row">
                  <div class="col-md-12">
                      <cards></cards>
                  </div>
              </div>
          </div>
          <div class="container-flex my-charts" style="background-color:#FFFFFF">
              <div class="row" style="justify-content: space-around; margin-left:70px;">
                  <div class="col-md-6">
                      <graph></graph>
                  </div>
                  <div class="col-md-4">
                      <pie></pie>
                  </div>
              </div>
          </div>
          <div class="container-flex">
              <div class="class">
                  <dic class="col-md-6">
                      <customer-details></customer-details>
                  </dic>
              </div>
          </div>
      </div>-->
      <div class="container-flex app-cards">
              <div class="row">
                  <div class="col-md-12">
                      <cards></cards>
                  </div>
              </div>
          </div>
           <div class="container-flex my-charts" style="background-color:#FFFFFF">
              <div class="row" style="justify-content: space-around; margin-left:70px;">
                  <div class="col-md-6">
                      <graph></graph>
                  </div>
                  <div class="col-md-4">
                      <pie></pie>
                  </div>
              </div>
          </div>
            <div class="container-flex">
              <div class="">
                  <dic class="col-md-6">
                      <customer-details></customer-details>
                  </dic>
              </div>
          </div>
    </div> 
</template>

<script>
import Header from './shared/Header.vue'
import Nav from './shared/Nav.vue'
import Cards from './private/Cards.vue'
import CustomerDetails from './private/CustomerDetails.vue'
import Graph from './private/Graph.vue'
import Pie from './private/Pie.vue'
export default {
    components: {
            appHeader:Header,
            appNav: Nav,
            cards: Cards,
            customerDetails: CustomerDetails,
            graph:Graph,
            pie:Pie
        }
}
</script>
<style scoped>
    .left{
        float:left;
        width: 5%;
        background-color: black;
        text-align: center;
        height:100%;
        position: fixed;
        z-index: 1;
    }
    .right{
        float:right;
        width: 95%;
        height:100%;
        background-color: #F7F7F8;
    }
    .app-header{
        margin-bottom: 50px;
    }
    .app-cards{
        margin-bottom: 50px;
    }
    .my-charts{
        margin-bottom: 50px;
    }
</style>