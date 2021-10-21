<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <HomeRen msg="Welcome to Your Vue.js App"/>
    <ShopWithUs/>

  </div>
</template>

<script>
// @ is an alias to /src
import HomeRen from '@/components/Home/HomeRen.vue'
import ShopWithUs from '@/components/Home/ShopWithUs.vue'

export default {
  name: 'Home',
  components: {
    HomeRen,
    ShopWithUs
  }
}
</script>
