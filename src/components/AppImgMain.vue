<script>
export default {
  name: 'AppImgMain',
}
</script>

<template>

<div>
    <img src="../assets/buy-comics-digital-comics.png" alt="Logo">
    <span>DIGITAL COMICS</span>
</div>
<div>
    <img src="../assets/buy-comics-merchandise.png" alt="Logo">
    <span>DC MERCHANDISE</span>
</div>
<div>
    <img src="../assets/buy-comics-subscriptions.png" alt="Logo">
    <span>SUBSCRIPTION</span>
</div>
<div>
    <img src="../assets/buy-comics-shop-locator.png" alt="Logo">
    <span>COMIC SHOP LOCATOR</span>
</div>
<div>
    <img class="img-main" src="../assets/buy-dc-power-visa.svg" alt="Logo">
    <span>DC POWER VISA</span>
</div>
</template>

<style lang="scss" scoped>
    
    div{
        display: flex;
        align-items: center;       
    }
    span{
        padding: 10px;
        color: white;
    }
    img{
        max-width: 50px;
        max-height: 50px;

    }
</style>