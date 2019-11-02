<template>
    <div>
        <div class="vertical-menu">
            <router-link to="#"><i class="fa fa-bars fa-2x" aria-hidden="true"></i></router-link>
            <router-link to="/"><i class="fa fa-home fa-2x" aria-hidden="true"></i></router-link>
            <router-link to="#"><i class="fa fa-file fa-2x" aria-hidden="true"></i></router-link>
            <router-link t0="#"><i class="fa fa-search fa-2x" aria-hidden="true"></i></router-link>
            <router-link to="#"><i class="fa fa-area-chart fa-2x" aria-hidden="true"></i></router-link>
            <router-link to="#"><i class="fa fa-inbox fa-2x" aria-hidden="true"></i></router-link>
            <router-link to="#"><i class="fa fa-file-video-o fa-2x" aria-hidden="true"></i></router-link>
            <router-link to="#"><i class="fa fa-calendar fa-2x" aria-hidden="true"></i></router-link>
            <router-link to="#"><i class="fa fa-users fa-2x" aria-hidden="true"></i></router-link>
            <router-link to="#"><i class="fa fa-cog fa-2x" aria-hidden="true"></i></router-link>
        </div>
    </div>
</template>
<script>

export default {

}
</script>
<style  scoped>
.fa{
    padding: 5px 0 5px 0;
}
.vertical-menu a {
  color: white; 
  display: block;  
  text-decoration: none; 
  margin-top:20px;
  margin-bottom: 35px;
  height: 100%;
}
.vertical-menu a:hover{
    background-color:#5A5A5B;
}

</style>