<script>
import AppImgMain from './AppImgMain.vue';
export default {
  name: 'AppMain',
  components:{
    AppImgMain
  },
}
</script>

<template>  
  <main>
    <div class="background-black">
      <h1 class="container">Content goes here</h1>
    </div>
    <div class="main-top">
      <section class="container ">
        <AppImgMain/>
      </section>
    </div>
  </main>
</template>

<style lang="scss" scoped>
.background-black{
  background-color: black;
}
    h1{
      
      color: white;
      padding: 30px;
    }
    .main-top{
      background-color: #0282f9;
      .container{
        display: flex;
        justify-content: space-between;
        padding: 30px 0 30px;
      }
    }

</style>