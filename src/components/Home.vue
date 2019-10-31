<template>
    <div id="content">
      <!-- <div class="content">
        <div class="header right"><app-header></app-header></div>
        <div class= "nav left"><app-nav></app-nav></div>
        <div class="main-content right">
        <div class="cards  same"><cards></cards></div> 
        <div class="main  same"><customer-details></customer-details></div>
        </div> 
       </div> -->
       <div class="move-left">
           <div class="my-nav">
               <app-nav></app-nav>
           </div>
       </div>
       <div class="move-right">
           <div class="my-header">
               <app-header>
               </app-header>
           </div>
           <div class="cards"><cards></cards></div> 
           <div class="temp"></div>
           <div class=" charts row">
               <div class="col-md-1"></div>
               <div class="col-md-6 a"><graph></graph></div>
                 <div class="col-md-3 a"><pie></pie></div>
               
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
#content{
    width: 80%;
    margin:auto; 
    }
.temp{
    content: "";
    clear: both;
    display: block;
}
.move-left{
    float:left;
    width: 10%;
}
a{
    
        background-color: darkkhaki;
    
}
.move-right{
    float: right;
    width:97%;
    height:100%;
}
.my-nav{
    background-color: aquamarine;
    position: fixed;
    z-index:1;
    overflow: hidden;
    height:100%;
    z-index: 1;
    border: 1px solid black;
}
.my-header{
    border:1px solid black;
    width: 100%;
}
.cards{
    margin:20px;
}
 /*.left{
     float: left;
 }
 .nav{
     width: 10%;
     overflow: hidden;
     height:100%;
     position: fixed;
     background-color: #eee; 
     z-index: 1;
     border: 1px solid black;
 }
 .header{
     width: 90%;
     height:80px;
     border: 1px solid black;
 }
 .right{
     float:right;
 }
 .cards{
     width: 90%;
     margin: 30px 0px 30px 0px;
     display: flex;
 }
 .main{
     width: 90%;
     display: flex;
 }
.content{
    width: 80%;
    margin: auto;
}
.main-content{
    width: 90%;
    height:100%;
    background-color: black;
} */
</style>