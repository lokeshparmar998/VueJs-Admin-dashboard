<template>
    <div>
        <div class="my-header">
            <div class="container-flex">
                <div class="row">
                    <div class="account col-md-2">
                        <h4>{{name}}</h4>
                        <p> Account Setting</p>
                    </div>
                    <div class="account-setting col-md-1">
                        <i class="fa fa-user-circle-o fa-3x account" aria-hidden="true"></i>
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
.my-header{
    background-color: #FFFFFF;
}
    .row{
        justify-content: flex-end;
        align-items: center;
    }
</style>