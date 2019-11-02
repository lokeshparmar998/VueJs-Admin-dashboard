<template>
  <div>
     <div class="left">
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
          <router-view></router-view>
          </div>
    <!--<app-home></app-home> -->
  </div>
</template>

<script>
import Header from './components/shared/Header'
import Nav from './components/shared/Nav.vue'
export default {
  components:{
    appHeader: Header,
    appNav:Nav
  }
}
</script>

<style>
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
</style>
