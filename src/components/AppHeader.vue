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
          {
            text: 'CHARACTERS',
            active: true,
          },
          {
            text: 'COMICS',
            active: false,
          },
          {
            text: 'MOVIES',
            active: false,
          },
          {
            text: 'TV',
            active: false,
          },
          {
            text: 'GAMES',
            active: false,
          },
          {
            text: 'COLLECTIBLES',
            active: false,
          },
          {
            text: 'VIDEOS',
            active: false,
          },
          {
            text: 'FANS',
            active: false,
          },
          {
            text: 'NEWS',
            active: false,
          },
          {
            text: 'SHOP',
            active: false,
          },   
        ]
    }
  },
  methods: {
    changeColor(index){
      this.links.forEach((elm, i)=>{
        if(index === i){
          elm.active=true;
        }else{
          elm.active=false;
        }
      });
    },
  },
};
</script>

<template>
  <header class="container">
        <AppLogo/>
        <nav class="main-nav">
            <ul>
                <li 
                  v-for="(link, index) in links" 
                  :class="{active: link.active}" 
                  @click="changeColor(index)"
                >
                  <a href="#">{{link.text}}</a>
                </li>
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
            li{
              &.active {
                    color: #0282f9;
                    border-bottom: 3px solid #0282f9;
                }
            }
            a {
                font-size: 13px;
                display: inline-block;
                padding: 15px 25px;
                text-decoration: none;
                color: #000;               
            }
        }
    }
}
</style>
