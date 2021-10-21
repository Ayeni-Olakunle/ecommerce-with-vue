<template>
    <b-container fluid class="bv-example-row" style="height: 500px;padding-top: 50px;margin-bottom: 100px;">
        <h1 class="shop">SHOP With <span class="us">US</span></h1>
        <p class="pick">Handpicked Favourites just for us</p>
        <b-row>
            <b-col sm="2">
                <div style="text-align: center;">
                    <div>
                        <div class="product">
                            <div class="holdProduct">
                                <p>Product</p>
                            </div>
                            
                        </div>
                        <div>
                            <img v-bind:src="require('@/assets/bag.jpg')" id="image"/>
                        </div>
                    </div>
                    <div>
                        <p class="info">Hands Bags</p>
                    </div>
                        
                </div>
            </b-col>
            <b-col sm="2">
                <div style="text-align: center;">
                    <img v-bind:src="require('@/assets/watch.jpg')" id="image"/>
                    <div>
                        <p class="info">Watches</p>
                    </div> 
                </div>
            </b-col>
            <b-col sm="2">
                <div style="text-align: center;">
                    <img v-bind:src="require('@/assets/shoe.jpg')" id="image"/>
                    <div>
                        <p class="info">Shoe</p>
                    </div>
                        
                </div>
            </b-col>
            <b-col sm="2">
                <div style="text-align: center;">
                    <img v-bind:src="require('@/assets/suit2.jpg')" id="image"/>
                    <div>
                        <p class="info">Suits</p>
                    </div>
                        
                </div>
            </b-col>
            <b-col sm="2">
                <div style="text-align: center;">
                    <img v-bind:src="require('@/assets/accessories.jpg')" id="image"/>
                    <div>
                        <p class="info">Things</p>
                    </div>
                        
                </div>
            </b-col>
            <b-col sm="2">
                <div style="text-align: center;">
                    <img v-bind:src="require('@/assets/fragrance.jpg')" id="image"/>
                    <div>
                        <p class="info">Fragrance</p>
                    </div>
                        
                </div>
            </b-col>
        </b-row>
    </b-container>
</template>
<script>
export default {
    data(){
        return{

        }
    }
}
</script>
<style scoped>
.shop{
    text-align: center;
    font-size: 50px;
    font-weight: bolder;
}
.us{
    color: orangered;
}
.pick{
    text-align: center;
    color: gray;
    font-size: 18px;
    margin-bottom: 100px;
}
#image{
    width: 100%;
    height: 200px;
    border-radius: 50%;
}
.info{
    font-size: 22px;
    font-weight: bold;
    margin-top: 20px;
}
.holdProduct{
    background-color: #00000082;
    width: 70%;
    margin-left: -30px;
    height: 150px;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 22px;
    color: white;
    font-weight: bold;
    cursor: pointer;
    visibility: hidden;
    
}
.holdProduct:hover{
    visibility: visible;
}
.product{
    position: absolute;
    width: 100%;
    height: 200px;
    display: flex;
    justify-content: center;
    align-items: center;
}

</style>