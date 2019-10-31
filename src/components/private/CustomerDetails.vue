<template>
    <div>
        <div class="details" >
            <div class="customer" v-for="customer in customers" :key="customer" >
                {{customer.name}}
                {{customer.join}}
                {{customer.contact}} 
                {{customer.location}}
            </div>
        </div>
    </div>
</template>
<script>
export default {
    data: function(){
        return{
            customers:[
                {name:"Lokesh Parmar ", join:"11 Dec 2019", contact:9910191307, location:"India"},
                {name:"Test Customer ", join:"11 Dec 2019", contact:9910191307, location:"India"},
                {name:"Test Customer ", join:"11 Dec 2019", contact:9910191307, location:"India"},
                {name:"Test Customer ", join:"11 Dec 2019", contact:9910191307, location:"India"},
                {name:"Test Customer ", join:"11 Dec 2019", contact:9910191307, location:"India"},
                {name:"Test Customer ", join:"11 Dec 2019", contact:9910191307, location:"India"},
                {name:"Test Customer ", join:"11 Dec 2019", contact:9910191307, location:"India"},
            ]
        }
    }
}
</script>
<style scoped>
    .details{
        
        background-color: bisque;
    }
    .customer{
        padding: 10px;
        margin: 10px;

    }
  
</style>