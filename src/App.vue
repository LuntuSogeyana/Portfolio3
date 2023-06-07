<template>
    <Navbar/>
    <HomeView/>
    <Footer/>
</template>

<script>
  import Navbar from '@/components/Navbar.vue'
  import Footer from '@/components/Footer.vue'
  import HomeView from '@/views/HomeView.vue'

  export default {
    name: 'app',
    components: {
      Navbar, 
      HomeView,
      Footer
    }
  }
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Boogaloo&family=Inter:wght@400;700&display=swap');
#app {
  font-family: 'Boogaloo', cursive;
  /* font-family: 'poppins', sans-serif; */
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
