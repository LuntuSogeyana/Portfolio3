<template>
  <div class="frame-1">
    <div class="rectangle-1"></div>
    <div class="rectangle-10"></div>
    <div class="hi-i-am-luntu-sogeyana-a-web-developer">
      Hi, I am Luntu Sogeyana,<br />a Web Developer!
    </div>
    <img class="dsc-3496-removebg-2" src="https://i.postimg.cc/Hxv8CVdV/DSC-3496-removebg.png" />
  </div>
</template>

<script>
export default {
  name: 'HelloWorld'
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap');

.frame-1,
.frame-1 * {
  box-sizing: border-box;
}

.frame-1 {
  background: #ffffff;
  width: 1500px;
  height: 673px;
  position: relative;
  overflow: hidden;
}

.rectangle-1 {
  background: black;
  width: 1520px;
  height: 673px;
  position: absolute;
  left: 0px;
  top: 0px;
}

.navigation {
  position: absolute;
  inset: 0;
}

.about,
.projects,
.testimonials,
.contact-me,
.home {
  color: #000000;
  text-align: left;
  font: 400 20px "Inter", sans-serif;
  position: absolute;
  top: 43px;
}

.about {
  left: 1067px;
}

.projects {
  left: 1220px;
}

.testimonials {
  left: 1373px;
}

.contact-me {
  left: 1525px;
}

.home {
  left: 915px;
}

.rectangle-10 {
  background: rgb(62, 61, 61);
  border-radius: 10px;
  border-style: solid;
  border-color: yellow;
  border-width: 1px;
  width: 1250px;
  height: 513px;
  position: absolute;
  left: 159px;
  top: 80px;
}

.hi-i-am-luntu-sogeyana-a-web-developer {
  color: yellow;
  text-align: left;
  font-family: 'Inter', sans-serif;
  font-weight: bold;
  font-style: italic;
  font-family: 'Inter';
  font-size: 44px;
  position: absolute;
  left: 620px;
  top: 259px;
  width: 586px;
  height: 164px;
}

.dsc-3496-removebg-2 {
  width: 533px;
  height: 751px;
  position: absolute;
  left: 50px;
  top: -81px;
}
</style>


