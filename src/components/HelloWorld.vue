<template>
  <div class="hello">
    <div class="header">
      <div class="logo">
        <img src="./../assets/logo.png" alt="">
      </div>
      <div class="nav">
          <router-link :to="{ name: '', params: {} }"><div>WORKS</div></router-link>
          <router-link :to="{ name: '', params: {} }"><div>News</div></router-link>
          <router-link :to="{ name: '', params: {} }"><div>Thinking</div></router-link>
          <router-link :to="{ name: '', params: {} }"><div>About us</div></router-link>
      </div>
    </div>
    <div class="banner">
      <img src="./../assets/banner.jpg">
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.header, .banner{
  width: 87.6%;
  margin: 0 auto;
  margin-top: 36px;
}
.header{
  display: flex;
  justify-content:space-between;
}
img{
  width: 100%;
  height: 100%;
}
.logo{
width: 20%;
}
.nav{
  display: flex;
}
.nav div{
  padding: 20px 10px 0px 10px;
}
.nav div::after{
  width: 1px;
  background: #000000;
}
</style>
