<template>
    <div>
        <div class="container-flex">
            <div class="row" style="justify-content: space-around;">
                <div class="col-md-3 exp">
                     <div class="container">
                         <div class="row item">
                             <div class="col-md-8">
                                 <h3>Total sale</h3>
                                    <p >{{totalSale}}</p>
                             </div>
                             <div class="col-md-2" style="color:#FF9500">
                                <i class="fa fa-credit-card-alt fa-2x" aria-hidden="true"></i>
                             </div>
                         </div>
                     </div>
                </div>
                <div class="col-md-3 exp">
                     <div class="container">
                         <div class="row item">
                             <div class="col-md-8">
                                 <h3>Total Income</h3>
                                    <p >{{totalIncome}}</p>
                             </div>
                             <div class="col-md-2" style="color:#FB404B">
                                 <i class="fa fa-tags fa-2x" aria-hidden="true"></i>
                             </div>
                         </div>
                     </div>
                </div>
                <div class="col-md-3 exp">
                     <div class="container">
                         <div class="row item">
                             <div class="col-md-8">
                                 <h3>Total Views</h3>
                                    <p >{{totalViews}}</p>
                             </div>
                             <div class="col-md-2">
                                <i class="fa fa-desktop fa-2x" aria-hidden="true"></i>
                             </div>
                         </div>
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
            totalSale: 12991,
            totalIncome:23523,
            totalViews:39823
        }
    }
}
</script>
<style scoped>
    .exp{
    
        border: 0.15px solid lightgray;
        background-color: #FFFFFF  
    } 
    .item{
        text-align: center;
        align-items: center;
    }
    .spaceme{
        justify-content: space-between;
    }
</style>