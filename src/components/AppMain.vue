<script>
import AppImgMain from './AppImgMain.vue';
import SectionCard from './SectionCard.vue';
export default {
  name: 'AppMain',
  components:{
    AppImgMain,
    SectionCard
  },
}
</script>

<template>  
  <main>
    <div class="hero">
      
    </div>
    <div class="background-color">
      <div>
        <h1 class="container">Content goes here</h1>
      </div>
    </div>
    <div class="background-color">
      <div class="container">
        <SectionCard/>
      </div>
    </div>
    <div class="main-bottom">
      <section class="container ">
        <AppImgMain/>
      </section>
    </div>
  </main>
</template>

<style lang="scss" scoped>
.hero{
  background-image: url(../assets/jumbotron.jpg);
  height: 400px;
  background-size: cover;
  background-repeat: no-repeat;
}
.background-color{
  background-color: #1c1c1c;
}

    h1{
      
      color: white;
      padding: 30px;
    }
    .main-bottom{
      background-color: #0282f9;
      .container{
        display: flex;
        justify-content: space-between;
        padding: 30px 0 30px;
      }
    }

</style>