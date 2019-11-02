<template>
    <div>
        <div class="my-header">
            <div class="container-flex">
                <div class="row">
                    <div class="account col-md-2">
                        <h4>{{name}}</h4>
                            <router-link to="#">Account Setting</router-link>
                    </div>
                    <div class="account-setting col-md-1">
                        <router-link to="#" style="color:gray"><i class="fa fa-user-circle-o fa-3x account" aria-hidden="true"></i></router-link>
                    </div>  
                </div>
            </div>
           
        </div>
                  
    </div>
</template>
<script>
export default {
    data: function(){
        return{
            name: "Lokesh Parmar"
        }
    }
}
</script>
<style scoped>
.account{
    margin: 0px;
    padding: 0px;

}
.account-setting{
    margin: 0px;
    padding: 0px;
    
}
a{
    text-decoration: none;
}
.my-header{
    background-color: #FFFFFF;
}
    .row{
        justify-content: flex-end;
        align-items: center;
    }
    .fa:hover{
       color:#EF106F;
    }
</style>