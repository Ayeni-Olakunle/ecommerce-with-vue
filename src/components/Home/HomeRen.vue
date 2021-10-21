<template>
    <div id="LandingPage">
        <b-container fluid class="bv-example-row holdHome">
            <b-row>
                <b-col sm="7" class="holdSeven">
                    <div class="holdSevens">
                        <img v-bind:src="require('@/assets/' + ImagValue)" id="image"/>
                        <div>
                            <p class="discount">WOMEN'S FASHION<br>50% OFF</p>
                            <button class="shopNow">Shop Now</button>
                        </div>
                        
                    </div>
                </b-col>
                <b-col sm="5" class="holdFive">
                    <div class="rightBar">
                        <div class="men">
                            <div>
                                <p class="discount">MEN'S<br>FASHION<br>50%<br>OFF</p>
                            </div>
                        </div>
                    </div>
                </b-col>
            </b-row>
            </b-container>
            <div>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            text: "working",
            ImagValue: 'fashion1.jpg',
            count:0
        }
    },
    mounted() {
    setInterval(() => {
        let ImageList = ["fashion1.jpg", "fashion2.jpg", "fashion3.jpg", "fashion4.jpg", "fashion5.jpg", "fashion6.jpg"]
        this.ImagValue = ImageList[this.count]
        if (this.count==6) {
            this.count=0
        }
        this.count++
    }, 4000)
  }


}
</script>

<style scoped>
.shopNow{
    margin-left: 25px;
    padding: 10px 20px;
    border: none;
    background-color: white;
    color: orangered;
    font-weight: 700;
    font-size: 20px;
}
#image{
    width: 100%;
    height: 700px;
    position: absolute;
    z-index: -1;
}
.holdSeven{
    padding: 0;
}
.holdSevens{
    height: 700px;
    width: 100%;
    background-position: center;
    background-size: cover;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #00000073;
}
.holdSeven{
    height: 700px;
    width: 100%;
}
.holdFive{
    padding: 0;
}

.rightBar{
  background-image: url("https://images.unsplash.com/photo-1595238793138-caeffc776186?ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTF8fG1hbiUyMGluJTIwc3VpdCUyMHdpdGglMjBibGFjayUyMGJhY2tncm91bmR8ZW58MHx8MHx8&ixlib=rb-1.2.1&w=1000&q=80");
  height: 700px;
  width: 100%;
  background-position: center;
  background-size: cover;
}
.men{
  display: flex;
  width: 100%;
  height: 100%;
  align-items: center;
}
</style>