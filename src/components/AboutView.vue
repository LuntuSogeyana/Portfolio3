<template>
  <h1>About Me</h1>
  <div class="blue-line"></div>
  <div id="about" class="about-section" data-aos="fade-up" data-aos-duration="1000">
    <h2 class="section-title">My skills and value as a developer</h2>
    <div class="skills">
      <div class="skill">
        <i class="fab fa-html5 fa-bounce" style="--fa-animation-delay: 0.1s; --fa-animation-duration:2.3s;"></i>
        <span>HTML5</span>
        <div class="hidden">Started learning HTML5 on September 2022</div>
      </div>
      <div class="skill">
        <i class="fab fa-css3 fa-bounce" style="--fa-animation-delay: 0.3s; --fa-animation-duration:2.3s;"></i>
        <span>CSS</span>
        <div class="hidden">Proficient in CSS styling</div>
      </div>
      <div class="skill">
        <i class="fab fa-bootstrap fa-bounce" style="--fa-animation-delay: 0.5s; --fa-animation-duration:2.3s;"></i>
        <span>Bootstrap</span>
        <div class="hidden">Experience with Bootstrap framework</div>
      </div>
      <div class="skill">
        <i class="fab fa-js fa-bounce" style="--fa-animation-delay: 0.7s; --fa-animation-duration:2.3s;"></i>
        <span>JavaScript</span>
        <div class="hidden">Skilled in JavaScript programming</div>
      </div>
      <div class="skill">
        <i class="fab fa-vuejs fa-bounce" style="--fa-animation-delay: 0.9s; --fa-animation-duration:2.3s;"></i>
        <span>Vue.js</span>
        <div class="hidden">Experience with Vue.js framework</div>
      </div>
      <div class="skill">
        <i class="fas fa-database fa-bounce" style="--fa-animation-delay: 1.1s; --fa-animation-duration:2.3s;"></i>
        <span>MySQL</span>
        <div class="hidden">Proficient in MySQL database</div>
      </div>
      <div class="skill">
        <i class="fab fa-node-js fa-bounce" style="--fa-animation-delay: 1.3s; --fa-animation-duration:2.3s;"></i>
        <span>Node.js</span>
        <div class="hidden">Experience with Node.js backend development</div>
      </div>
      <div class="skill">
        <i class="fab fa-wordpress fa-bounce" style="--fa-animation-delay: 1.5s; --fa-animation-duration:2.3s;"></i>
        <span>WordPress</span>
        <div class="hidden">Skilled in WordPress development</div>
      </div>
      <div class="skill">
        <i class="fab fa-php fa-bounce" style="--fa-animation-delay: 1.7s; --fa-animation-duration:2.3s;"></i>
        <span>PHP</span>
        <div class="hidden">Experience with PHP programming</div>
      </div>
      <div class="skill">
        <i class="fab fa-python fa-bounce" style="--fa-animation-delay: 1.9s; --fa-animation-duration:2.3s;"></i>
        <span>Python</span>
        <div class="hidden">Learned Python</div>
      </div>
      <div class="skill">
        <i class="fab fa-react fa-bounce" style="--fa-animation-delay: 2.2s; --fa-animation-duration:2.3s;"></i>
        <span>React</span>
        <div class="hidden">Learned React</div>
      </div>
    </div>
    <p class="description">As a skilled web developer, my value lies in my experience, versatility, and dedication to continuous learning. My ability to work efficiently, meet deadlines, and maintain quality work allows me to create unique, simple, and efficient websites that meet the needs of various user tastes. By keeping up with the latest web trends and development techniques, I provide unique solutions that help differentiate my work from the competition.</p>
  </div>
</template>

<style>
@import '~@fortawesome/fontawesome-free/css/all.css';

.about-section {
  border-radius: 15px;
  background-color: rgb(62, 61, 61);
  padding: 20px;
  margin-top: 50px;
  margin-left: 5vw;
  width: 90vw;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  color: yellow;
}

h1 {
  margin-top: 50px !important;
  color: white;
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
  font-weight: bolder;
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
  position: relative;
  flex: 1 1 150px; /* Allows items to grow and shrink */
  max-width: 200px; /* Maximum width of each skill item */
}

.skill i {
  font-size: 80px;
  margin-right: 20px;
  color: black;
  opacity: 60%;
}

.skill:hover .fa-html5 {
  color: orangered;
}

.skill:hover .fa-css3 {
  color: rgb(67, 100, 233);
}

.skill:hover .fa-bootstrap {
  color: rgb(190, 40, 190);
}

.skill:hover .fa-js {
  color: orange;
} 
/* checking */

.skill:hover .fa-vuejs {
  color: green;
}

.skill:hover .fa-database {
  color: lightblue;
}

.skill:hover .fa-node-js {
  color: darkgreen;
}

.skill:hover .fa-wordpress {
  color: rgb(109, 109, 210);
}

.skill:hover .fa-php {
  color: rgb(75, 138, 202);
}

.skill:hover .fa-python {
  color: purple;
}

.skill span {
  font-size: 28px;
  font-weight: bold;
}

.description {
  font-size: 30px;
  font-weight: 600;
  line-height: 1.5;
  text-align: center;
  color: white;
  margin: 0 20px; /* Add some side margins for better spacing */
}

.hidden {
  display: none;
  position: absolute;
  top: -50px;
  left: 50%;
  transform: translateX(-50%);
  background-color: rgb(50,50, 50);
  color: white;
  padding: 8px;
  border-radius: 4px;
  box-shadow: 0 2px 5px black;
  z-index: 2;
  opacity: 0;
  transition: opacity 0.3s ease-in-out;
  width: 200px;
  font-size: 14px;
  font-weight: bold;
  text-align: center;
}

.hidden::before {
  content: "";
  position: absolute;
  top: 100%;
  left: 50%;
  transform: translateX(-50%);
  border-style: solid;
  border-width: 10px 10px 0 10px;
  border-color: rgb(50, 50, 50) transparent transparent transparent;
}

.skill:hover .hidden {
  display: block;
  opacity: 1;
}

@media screen and (max-width: 1200px) {
  .about-section {
    padding: 20px;
    margin-left: 20px;
    margin-right: 20px;
    width: auto;
    height: auto;
    min-height: 100vh;
    overflow-x: hidden;
  }

  .section-title {
    font-size: 48px;
    margin-bottom: 20px;
  }

  .skills {
    margin-bottom: 30px;
  }

  .skill i {
    font-size: 70px;
    margin-right: 15px;
  }

  .skill span {
    font-size: 24px;
  }

  .description {
    font-size: 24px;
  }
}

@media screen and (max-width: 768px) {
  .about-section {
    padding: 15px;
    margin-left: 10px;
    margin-right: 10px;
    width: auto;
    height: auto;
    min-height: 100vh;
    overflow-x: hidden;
  }

  .section-title {
    font-size: 36px;
    margin-bottom: 15px;
  }

  .skills {
    margin-bottom: 20px;
  }

  .skill i {
    font-size: 60px;
    margin-right: 10px;
  }

  .skill span {
    font-size: 20px;
  }

  .description {
    font-size: 18px;
  }
}

</style>



