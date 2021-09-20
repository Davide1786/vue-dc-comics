<template>
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
    display: flex;
    justify-content: space-around;
    align-items: center;


    ul {
      list-style: none;
      display: flex;

      li a {
        text-decoration: none;
        padding: 20px;
        text-transform: uppercase;  
        color: $colore-link;

        &:hover,
        &.active {
          color: $cambio-colore;
        }

      }

    }

  }

 
</style>
