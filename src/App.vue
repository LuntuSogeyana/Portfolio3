<template>
    <Navbar/>
    <HomeView/>
    <Footer/>
    <CustomCursor/>
</template>

<script>
  import Navbar from '@/components/Navbar.vue'
  import Footer from '@/components/Footer.vue'
  import HomeView from '@/views/HomeView.vue'
  import CustomCursor from './components/CustomCursor.vue'

  export default {
    name: 'app',
    components: {
      Navbar, 
      HomeView,
      Footer,
      CustomCursor,
    }
  }
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100&display=swap');
#app {
  font-family: 'Montserrat', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

body {
  cursor: none !important;
}

button {
  cursor: none !important;
}

body:hover {
  cursor: none;
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
