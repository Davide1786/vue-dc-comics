<template>
  <div>
    <div class="barra-nera">
      <h3 class="goes">Content goes here</h3>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MainTop',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../components/Style/Variabili';

  .barra-nera {
    width: 100%;
    height: 120px;
    display: flex;
    align-items: center;
    background: black;

      .goes{
        width: 70%;
        margin: 0 auto;
        color: white;
        font-size: 28px;
        font-weight: 900;
      }
  }

 
</style>
