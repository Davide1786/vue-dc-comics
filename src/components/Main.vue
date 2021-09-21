<template>
  <div class="barra">
    <div class="barra-nera">
    <Fumetti 
      v-for="(item, index) in fumetti"
      :key="index"
      :it="item"
    />
    </div>


  </div>
</template>

<script>

import Fumetti from '@/components/Fumetti.vue';
import dcComics from '@/assets/data/dcComics.js';
export default {
  name: 'Main',
  components: {
    Fumetti
  },
  data() {
    return {
      fumetti: dcComics
    }

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../components/Style/Variabili';

  .barra {
    width: 100%;
    height: 600px;
    display: flex;
    align-items: center;
    background: black;

      .barra-nera{
        width: 70%;
        height: 80%;
        margin: 0 auto;
        display: flex;
        flex-wrap: wrap;
        background: olivedrab;
      }
  }

 
</style>
