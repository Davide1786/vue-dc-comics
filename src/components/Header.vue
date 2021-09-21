<template>
  <div>
    <div class="menu-navigazione">
      <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <nav>
        <ul class="navigatore">
          <li v-for="(link, index) in links" :key="index">
            <a :class="(link.current) ? 'active' : null" :href="link.url"> {{link.text}} </a>
          </li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      links: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "Tv",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../components/Style/Variabili';

  .menu-navigazione {
    width: 70%;
    margin: 0 auto;
    padding-top: 10px;
    height: 120px;
    display: flex;
    justify-content: space-between;
    align-items: center;


    ul {
      list-style: none;
      display: flex;
      li a {
        text-decoration: none;
        padding: 10px;
        text-transform: uppercase;  
        color: $colore-link;
        padding-bottom: 41px;
        &:hover,
        &.active {
          color: $cambio-colore;
          border-bottom: 5px solid #077CEA;
        }
      }
    }
  }

 
</style>
