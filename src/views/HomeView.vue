<template>
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

export default {
  name: 'HomeView',
  components: {
    HelloWorld,
    AboutView,
    Projects,
    Testimonials,
    Contact
  }
}
</script>

<style>
body {
  background-color: black;
}
</style>
