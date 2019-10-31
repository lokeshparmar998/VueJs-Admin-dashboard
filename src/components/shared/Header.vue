<template>
    <div>
        <div class="header-content">
            <div id="head">
                <div class="dsp">
                   <h2>{{name}}</h2>
                    <p> Account Setting</p>
                    </div>
                    <i class="fa fa-user-circle-o fa-3x account" aria-hidden="true"></i>
                
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

.header-content {
    
    text-align: center;
    padding: 20px;
    background: aquamarine;
    display: flex;
    justify-content: flex-end;
}

#head{
   display: flex;
    justify-content: space-around;
    margin-right: 3%; 
}

h2{
     min-width: -webkit-fill-available;
    
}

.account{
        margin-left: 15px;
}

p{
    float: right;
}
</style>