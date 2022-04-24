<template>
  <div id="app">
    
    <div class="container">
      <img src="./assets/logo-rmvbg.png" alt="logo">

      <div >     
        <nav>
          <router-link to="/">Home</router-link> |
          <router-link to="/about">Quem somos</router-link> |
          <router-link to="/projects">Projetos</router-link> |
          <router-link to="/contact">Fale conosco</router-link> 
        </nav>
      </div>
      <div class="social flex">
        <WhatsapLink />
        <InstaLink />
      </div>
    </div>


    <router-view/>
  </div>
</template>

<script>
import WhatsapLink from './components/WhatsapLink.vue'
import InstaLink from './components/InstaLink.vue'
export default {
  components: {
    WhatsapLink,
    InstaLink
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
 
 
}

.flex {
  display: flex;
}

.col {
  flex-direction: column;
}

.container {
        display: flex;
        align-items: center;
        justify-content: space-between;
        height: 200px;
        padding: 0 20px;
    }
    img {
        width: 180px;
    }

nav {
  

  a {
    text-decoration: none;
    font-weight: bold;
    color: #000000;


    &.router-link-exact-active {
      color: #631ed1;
    }

  
  }
  a:hover{
    color: #631ed1;
    
  }


}
</style>
