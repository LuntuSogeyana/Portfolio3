<template>
  <h1>About Me</h1>
  <div class="blue-line"></div>
  <div id="about" class="about-section" data-aos="fade-up" data-aos-duration="1000">
    <h2 class="section-title">My value as a developer</h2>
    <div class="skills">
      <div class="skill">
        <i class="fab fa-html5 fa-bounce" style="--fa-animation-delay: 0.1s; --fa-animation-duration:2.3s;"></i>
        <span>HTML5</span>
      </div>
      <div class="skill">
        <i class="fab fa-css3 fa-bounce" style="--fa-animation-delay: 0.2s; --fa-animation-duration:2.3s;"></i>
        <span>CSS</span>
      </div>
      <div class="skill">
        <i class="fab fa-bootstrap fa-bounce" style="--fa-animation-delay: 0.3s; --fa-animation-duration:2.3s;"></i>
        <span>Bootstrap</span>
      </div>
      <div class="skill">
        <i class="fab fa-js fa-bounce" style="--fa-animation-delay: 0.4s;--fa-animation-duration:2.3s;"></i>
        <span>JavaScript</span>
      </div>
      <div class="skill">
        <i class="fab fa-vuejs fa-bounce" style="--fa-animation-delay: 0.5s; --fa-animation-duration:2.3s;"></i>
        <span>Vue.js</span>
      </div>
      <div class="skill">
        <i class="fas fa-database fa-bounce" style="--fa-animation-delay: 0.6s; --fa-animation-duration:2.3s;"></i>
        <span>MySQL</span>
      </div>
      <div class="skill">
        <i class="fab fa-node-js fa-bounce" style="--fa-animation-delay: 0.7s; --fa-animation-duration:2.3s;"></i>
        <span>Node.js</span>
      </div>
      <div class="skill">
        <i class="fab fa-wordpress fa-bounce" style="--fa-animation-delay: 0.8s;--fa-animation-duration:2.3s;"></i>
        <span>WordPress</span>
      </div>
    </div>
    <p class="description">As a highly skilled web developer, my value lies in my extensive experience, versatility, and dedication to continuous learning. My ability to work efficiently, meet deadlines, and maintain high-quality work allows me to create unique and efficient websites that meet the needs of various customer tastes. By keeping up with the latest web trends and development techniques, I can provide cutting-edge solutions that help differentiate my clients from their competitors and attract new customers, ultimately driving business growth.</p>
  </div>
</template>

<script scoped>
export default {
  name: 'AboutView',
  mounted() {
    AOS.init();
  }
};
</script>



<style>
@import '~@fortawesome/fontawesome-free/css/all.css';

.about-section {
  border: 2px solid yellow;
  border-radius: 15px;
  /* outline: 2px solid yellow; */
  background-color: rgb(62, 61, 61);
  padding: 20px;
  margin-top: 50px;
  margin-left: 5vw;
  width: 90vw;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  /* font-family: Arial, sans-serif;  */
  color: yellow;
  /* box-shadow: 0px 5px 15px yellow; */
}

h1 {
  margin-top: 50px !important;
}

.blue-line {
  height: 0.3rem;
  width: 6rem;
  background-color: yellow;
  margin-bottom: calc(3rem + 2vmin);
  margin-left: auto;
  margin-right: auto;
}

.section-title {
  font-size: 60px;
  margin-bottom: 30px;
  text-align: center;
  font-weight: bold;
}

.skills {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  margin-bottom: 50px;
}

.skill {
  display: flex;
  align-items: center;
  margin: 10px;
  cursor: pointer;
}

.skill i {
  font-size: 80px;
  margin-right: 20px;
  color: black;
}

.skill:hover .fa-html5{
 color: orangered;
}

/* .skill:hover .fa-html5{ 
  animation: shake 150ms infinite;
  animation-timing-function: linear;   
} */

@keyframes shake {
  0% { transform: rotate(0.5deg); }
  50% { transform: rotate(-0.5deg); }
  100% { transform: rotate(0.5deg); }
}

.skill:hover .fa-css3{
 color: rgb(67, 100, 233);
}
.skill:hover .fa-bootstrap{
 color: rgb(190, 40, 190);
}
.skill:hover .fa-js{
 color: orange;
}
.skill:hover .fa-vuejs{
 color: green;
}
.skill:hover .fa-database{
 color: lightblue;
}
.skill:hover .fa-node-js{
 color: darkgreen;
}

.skill:hover .fa-wordpress{
 color: rgb(109, 109, 210);
}

.skill:nth-child(1):hover span {
  color: orangered !important;
}
.skill:nth-child(2):hover span {
  color: rgb(67, 100, 233) !important;
}
.skill:nth-child(3):hover span {
  color: rgb(190, 40, 190) !important;
}
.skill:nth-child(4):hover span {
  color: orange !important;
}
.skill:nth-child(5):hover span {
  color: green !important;
}
.skill:nth-child(6):hover span {
  color: lightblue !important;
}
.skill:nth-child(7):hover span {
  color: darkgreen !important;
}
.skill:nth-child(8):hover span {
  color: rgb(109, 109, 210) !important;
}

.skill span {
  font-size: 28px;
  font-weight: bold;
}

.description {
  font-size: 30px;
  line-height: 1.5;
  text-align: center;
}

@media screen and (max-width: 768px) {
  .about-section {
    margin-left: 20px;
    margin-right: 20px;
    width: auto;
    height: auto;
    min-height: 100vh;
    padding: 20px;
    overflow-x: hidden;

  }
  
  .section-title {
    font-size: 36px;
    margin-bottom: 20px;
  }
  
  .skills {
    margin-bottom: 30px;
  }
  
  .skill i {
    font-size: 60px;
    margin-right: 10px;
  }
  
  .skill span {
    font-size: 22px;
  }
  
  .description {
    font-size: 20px;
  }
}

</style>

