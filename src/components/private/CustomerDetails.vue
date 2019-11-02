<template>
    <div>
        <div class="container-flex details" >
            <div class="customer" v-for="customer in customers" :key="customer" >
               <div class="row">
                    <div class="col-md-3">
                    <h4>{{customer.name}}</h4>
                    
                </div>
                <div class="col-md-2">
                    <p> {{customer.join}}</p>
                    <p>Joined</p>
                </div>
                <div class="col-md-2">
                    <p> {{customer.contact}} </p>
                    <p>Phone Number</p>
                </div>
                <div class="col-md-2">
                     <p>{{customer.location}}</p>
                     <p>Location</p>
                </div>
                <div class="col-md-1">
                    <input type="button" value="Options" class="btn btn-primary">
                </div>
                <div class="col-md-1">
                    <input type="button" value="Details" class="btn btn-primary">
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
            customers:[
                {name:"Lokesh Parmar", join:"11 Dec 2019", contact:9910191307, location:"India"},
                {name:"Test Customer1", join:"11 Dec 2019", contact:9910191307, location:"India"},
                {name:"Test Customer2", join:"11 Dec 2019", contact:9910191307, location:"India"},
                {name:"Test Customer3", join:"11 Dec 2019", contact:9910191307, location:"India"},
                {name:"Test Customer4", join:"11 Dec 2019", contact:9910191307, location:"India"},
                {name:"Test Customer5", join:"11 Dec 2019", contact:9910191307, location:"India"},
                {name:"Test Customer6", join:"11 Dec 2019", contact:9910191307, location:"India"},
            ]
        }
    }
}
</script>
<style scoped>
.details{
    width: 80%;
    margin: 0 auto;
    border: 0.15px solid lightgray;
}
.customer{
    background-color: white;
    
    padding: 30px;
}
.customer:nth-child(even)
{
    background-color: aliceblue
}
</style>