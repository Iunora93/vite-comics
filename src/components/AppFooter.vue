<script>
export default {
  name: 'AppFooter',
}
</script>

<template>
  <section class="footer-top">
    <div class="container"></div>
  </section>

  <section class="footer-bottom">
    <div class="container">
      <div class="col-left">
        <button class="btn-footer">SIGN-UP NOW!</button>
      </div>
      <div class="col-right">
        <h4>FOLLOW US</h4>
        <img src="../assets/footer-facebook.png" alt="">
        <img src="../assets/footer-twitter.png" alt="">
        <img src="../assets/footer-youtube.png" alt="">
        <img src="../assets/footer-pinterest.png" alt="">
        <img src="../assets/footer-periscope.png" alt="">
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.footer-top{ 
  height: 400px;
  background-image: url(../assets/footer-bg.jpg);
  background-size: cover;  
  .container{
    background-image: url(../assets/dc-logo-bg.png);
    height: 100%;
    background-repeat: no-repeat;
    background-position: right;
  }
}
.footer-bottom{
  background-color: #303030;
  padding: 20px 20px;

  .container{
    display: flex;
    justify-content: space-between;
  }
  .btn-footer{
    color: white;
    background-color: #303030;
    border-color: #0282f9;
    padding: 20px;
  }
  .col-right{
    display: flex;
    align-items: center;
    justify-content: space-around;
    min-width: 400px;
    width: 30%;

    h4{
      color: #0282f9;
    }
  }
}
</style>