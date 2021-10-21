<template>
  <div id="app">
    <b-container fluid class="bv-example-row">
      <b-row>
        <b-col sm="12" style="position: absolute; z-index: 1000000000;">
          <div>
            <div class="userAndShop">
              <div>
                <p class="topoff">UPTO 30% OFF ON ALL STYLES, Click Here <b-icon icon="hand-index" scale="1" variant="light" style="transform: rotate(90deg);"></b-icon><SPan class="details"> for More Details</SPan></p>
              </div>
              <div>
                <p class="shopCart"><span class="user"><b-icon icon="person-fill" scale="1.8" variant="light" style="width: 20px;"></b-icon></span><span class="user" style="padding: 10px 20px;"><b-icon icon="cart-fill" scale="1.8" variant="light"></b-icon> My Cart</span></p>
              </div>
            </div>
            <div class="userAndShop" style="margin-top: 0;">
              <div>
                <p class="logo">SPRY<span class="details">S</span>TORE<span style="font-size: 20px; margin-left: 50px;"><b-icon icon="search" scale="1" variant="light" style="margin-right: 15px;"></b-icon>Search here</span></p>
              </div>
              <div>
                <b-navbar toggleable="lg" type="dark">
                  <!-- <b-navbar-brand href="#">NavBar</b-navbar-brand> -->

                  <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
                  <b-collapse id="nav-collapse" is-nav>
                    <b-navbar-nav>
                      <b-nav-item href="#">
                        <router-link to="/" class="linkxs menus">Home</router-link>
                      </b-nav-item>
                      <b-nav-item href="#">
                        <router-link to="/about" class="linkxs menus">About</router-link>
                      </b-nav-item>
                      <b-nav-item href="#">
                        <router-link to="/about" class="linkxs menus">What We Offer</router-link>
                      </b-nav-item>
                      <b-nav-item href="#">
                        <router-link to="/about" class="linkxs menus">Contact</router-link>
                      </b-nav-item>
                    </b-navbar-nav>
                  </b-collapse>
                </b-navbar>
              </div>
            </div>
          </div>
        </b-col>
      </b-row>
    </b-container>
    <div>
</div>
    <router-view/>
  </div>
</template>

<style>
.menus{
  color: white;
  font-size: 20px;
  margin: 0px 10px;
}
.menus:hover{
  color: rgb(168, 113, 11);
  font-size: 20px;
  margin: 0px 10px;
  text-decoration: none;
}
.shopCart{
  text-align: right;
  padding: 10px 20px;
  margin-bottom: 0;
  color: white;
}
.user{
  padding: 10px;
  background-color: #464646;
  border-radius: 90px;
  margin-right: 25px;
}

.user:hover{
  background-color: rgb(168, 113, 11);
  cursor: pointer;
}
.discount{
  color: white;
  font-size: 60px;
  line-height: 1;
  padding: 25px;
  font-weight: 600;
}
.userAndShop{
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 20px;
}
.topoff{
  font-size: 17px;
  font-weight: 400;
  color: white;
  margin-bottom: 0;
}
.details{
  color: orangered;
}
.logo{
  font-size: 30px;
  font-weight: 700;
  margin-bottom: 0;
  color: white;
}
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
} */
</style>
