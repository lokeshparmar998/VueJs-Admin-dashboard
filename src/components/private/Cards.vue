<template>
    <div>
       <div class="myCard">
            <div class="exp col-md-4">
                <div class="row">
                    <div class="col-md-8 sale"> 
                     <h3>Total sale</h3>
                        <p >21,340</p>
                        
                    </div>
                    <div class="col-md-4">
                            <i class="fa fa-shopping-bag fa-2x" aria-hidden="true"></i>
                        </div>
                </div>
           
            
        </div>
        <div class="exp col-md-4">
                <div class="row">
                    <div class="col-md-8 sale"> 
                     <h3>Total Income</h3>
                        <p >21,340</p>
                        
                    </div>
                    <div class="col-md-4">
                            <i class="fa fa-credit-card fa-2x" aria-hidden="true"></i>
                        </div>
                </div>
           
            
        </div>
         <div class="exp col-md-4">
                <div class="row">
                    <div class="col-md-8 sale"> 
                     <h3>Total Income</h3>
                        <p >21,340</p>
                        
                    </div>
                    <div class="col-md-4">
                            <i class="fa fa-television fa-2x" aria-hidden="true"></i>
                        </div>
                </div>
           
            
        </div>
        </div>  
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
    .exp{
        
        margin-left: 40px;
        height: 100px;
        width: 30%;
        border: 0.15px solid lightgray;
        flex-grow: 1;
        background-color: beige;
        text-align: center;
        float:left;
    } 

    .row{
        align-items: center;
    }

    .sale{
        margin-top: 16px;
    }
</style>