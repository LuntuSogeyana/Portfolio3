<template>
      <CustomCursor/>
      <HelloWorld/>
      <AboutView/>
      <Projects/>
      <Testimonials/>
      <Contact/>
</template>

<script>
import HelloWorld from '@/components/HelloWorld.vue'
import AboutView from '@/components/AboutView.vue'
import Projects from '@/components/Projects.vue'
import Testimonials from '@/components/Testimonials.vue'
import Contact from '@/components/Contact.vue'
// import CustomCursor from '@/components/CustomCursor.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld,
    AboutView,
    Projects,
    Testimonials,
    Contact,
}
}
</script>

<style>
body {
  background-color: black;
}

button {
  cursor: none !important;
}
</style>
