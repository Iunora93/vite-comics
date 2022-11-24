<script>
import AppLogo from './AppLogo.vue';
export default {
  name: 'AppHeader',
  components:{
    AppLogo
  },
  data() {
    return {
        links: [
            'CHARACTERS',
            'COMICS',
            'MOVIES',
            'TV',
            'GAMES',
            'COLLECTIBLES',
            'VIDEOS',
            'FANS',
            'NEWS',
            'SHOP'
        ]
    }
  }
}
</script>

<template>
  <header class="container">
        <AppLogo/>
        <nav class="main-nav">
            <ul>
                <li v-for="link in links"><a href="">{{link}}</a></li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
header {
  padding: 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    img{
      width: 70px;
    }
    .main-nav {  
        ul {
            display: flex;
            list-style: none;
            
            a {
                font-size: 12px;
                display: inline-block;
                padding: 15px 25px;
                text-decoration: none;
                color: #000;
                &.active {
                    background-color: var(--secondary-color);
                }
            }
        }
    }
}
</style>
