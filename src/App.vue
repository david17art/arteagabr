<template lang="html">
  <div id="app">
    <div class="row">
      <div class="col-md-6 offset-md-3">
        <div class="main">
          <div class="img animated bounce">
            <img src="./assets/logo.png" width="100%">
          </div>
          <hr>
          <h1 class="animated bounceInUp">Proximamente</h1>
          <a class="twitter-timeline" href="https://twitter.com/arteagabrca?ref_src=twsrc%5Etfw">Tweets by arteagabrca</a>
        </div>
      </div>
    </div>
    <footer>
        <div class="row justify-content-end">
          <div class="col-4">
            <ul class="social">
              <li><a href="https://facebook.com/arteagabr"><i class="fa fa-facebook"></i></a></li>
              <li><a href="https://twitter.com/arteagabrca"><i class="fa fa-twitter"></i></a></li>
              <li><a href="https://instagram.com/arteagabr"><i class="fa fa-instagram"></i></a></li>

            </ul>
          </div>
          <div class="col-4">
            <img width="50px" src="./assets/logo-rg.png">
          </div>
        </div>
    </footer>
  </div>
</template>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style lang="scss">
html {
  min-height: 100%;
  position: relative;
}
.social{
  display: inline-flex;
  list-style: none;
}
.social li{
  text-decoration: none;
  margin-right: 100px;
}
.social li a{
  color:#fff;
  font-size:1.8rem;
  text-decoration: none;
}
.social li a:hover{
  color:#d8d8d8;
}
.main{
  margin-top:5%;
}
.main hr{
  border-top: 10px solid #fff;
}
.main h1{
  font-size:3.5rem;
  color:#fff;
  text-align: center;
}
.main .img{
  margin-left:20%;
  margin-right: 20%;
}
footer{
  bottom:0;
  position:absolute;
  background:rgba(0,0,0,0.8);
  padding:10px;
  color: #fff;
  width: 100%;
}
body{
  margin-bottom: 15%;
    background:url("assets/background.jpg");
    /* Background image is centered vertically and horizontally at all times */
  background-position: center center;

  /* Background image doesn't tile */
  background-repeat: no-repeat;

  /* Background image is fixed in the viewport so that it doesn't move when
     the content's height is greater than the image's height */
  background-attachment: fixed;

  /* This is what makes the background image rescale based
     on the container's size */
  background-size: cover;
}

</style>
