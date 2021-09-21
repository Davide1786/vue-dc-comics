<template>
  <div class="slider-blu">
    <div class="w-70">
        <li class="special" v-for="(icon, index) in specials" :key="index">
          <img :src="require(`../assets/img/${icon.img}`)" alt="">
          {{ icon.titolo }}
        </li>
    </div>
  </div>
</template>

<script>
import Specials from '@/assets/data/Specials.js'
export default {
  name: 'MainBottom',
  data() {
    return {
      specials: Specials
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../components/Style/Variabili';

  .slider-blu {
    width: 100%;
    height: 200px;
    display: flex;
    align-items: center;
    background: #077CEB;
      li {
        list-style: none;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 14px;
        width: 100%;
        color: white;
        padding: 5px;
        
          img {
            height: 30%;
            margin-right: 10px;
          }
          // img[href$=".svg"] {
          //   height: 10%;
          // }
      }
  }

 
</style>
