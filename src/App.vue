<template>
  <div class="nav-container">
  <h1>Fylo</h1>
    <nav>
    <MobileNav></MobileNav>
  </nav>
</div>


<router-view/>
<FooterView/>
</template>
<script>
import FooterView from './components/FooterView.vue'
import MobileNav from './components/MobileNav.vue'
  export default {
    data() {
      return {
        
      }
    }, 
    methods: {
      handelView() {
        this.mobileView = window.innerWidth <= 990;
      }
    },
    components: {
      MobileNav,
      FooterView
      
    }
  }
</script>
<style>

* {
  flex-wrap: wrap;
}
.open {
    display: flex;
}
.main-span {
  display: flex;
  flex-direction: column;
  width: 30px;
  cursor: pointer;
}
.main-span span {
    width: 100%;
    height: 4px;
    background-color: #fff;
    margin-bottom: 3px;
    border-radius: 8px;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  
}
body {
  background-color: #1b2330;
}
.nav-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
}
h1 {
  color: #fff;
  font-size: 25px;
}

nav a {
  font-weight: bold;
  color: #fff;
}

nav a.router-link-exact-active {
  color: #42b983;
}



</style>
