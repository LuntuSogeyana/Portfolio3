<template>
  <div class="about-section">
    <h2 class="section-title">My value as a developer</h2>
    <div class="skills">
      <div class="skill">
        <i class="fab fa-html5"></i>
        <span>HTML5</span>
      </div>
      <div class="skill">
        <i class="fab fa-css3"></i>
        <span>CSS</span>
      </div>
      <div class="skill">
        <i class="fab fa-bootstrap"></i>
        <span>Bootstrap</span>
      </div>
      <div class="skill">
        <i class="fab fa-js"></i>
        <span>JavaScript</span>
      </div>
      <div class="skill">
        <i class="fab fa-vuejs"></i>
        <span>Vue.js</span>
      </div>
      <div class="skill">
        <i class="fas fa-database"></i>
        <span>MySQL</span>
      </div>
      <div class="skill">
        <i class="fab fa-node-js"></i>
        <span>Node.js</span>
      </div>
      <div class="skill">
        <i class="fab fa-wordpress"></i>
        <span>WordPress</span>
      </div>
    </div>
    <p class="description">As a highly skilled web developer, my value lies in my extensive experience, versatility, and dedication to continuous learning. My ability to work efficiently, meet deadlines, and maintain high-quality work allows me to create unique and efficient websites that meet the needs of various customer tastes. By keeping up with the latest web trends and development techniques, I can provide cutting-edge solutions that help differentiate my clients from their competitors and attract new customers, ultimately driving business growth.</p>
  </div>
</template>

<script>
export default {
  name: 'AboutView'
};
</script>

<style>
@import '~@fortawesome/fontawesome-free/css/all.css';

.about-section {
  border: 2px solid yellow;
  border-radius: 15px;
  outline: 2px solid yellow;
  background-color: rgb(62, 61, 61);
  padding: 20px;
  margin-left: 5vw;
  width: 90vw;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  color: yellow;
  box-shadow: 0px 5px 15px yellow;
}

.section-title {
  font-size: 48px;
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
}

.skill i {
  font-size: 80px;
  margin-right: 20px;
  color: black;
}

.skill span {
  font-size: 28px;
  font-weight: bold;
}

.description {
  font-size: 24px;
  line-height: 1.5;
  text-align: center;
}
</style>

