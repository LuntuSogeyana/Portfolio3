<template>
  <h1>Projects</h1>
  <div class="blue-line"></div>
<div id="projects" class="card-container"> 
  <div class="card" data-aos="fade-up" data-aos-duration="1000">
    <img class="card-image" src="../assets/Flip.png" alt="Card 2" />
    <div class="card-content">
      <h3 class="card-title">Flip-card</h3>
      <p class="card-description">A flip card of Monkey D. Luffy</p>
      <a class="card-link" href="https://silver-eclair-a67fc6.netlify.app/" target="_blank">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/flip--card.git" target="_blank">GitHub</a>
     </div>
  </div>

  <div class="card" data-aos="fade-up" data-aos-duration="1000">
    <img class="card-image" src="../assets/Animated-Calculator.png" alt="Card 1" />
    <div class="card-content">
      <h3 class="card-title">Calculator</h3>
      <p class="card-description">A simple calculator .</p>
      <a class="card-link" href="https://luntucalculator.netlify.app/" target="_blank">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/Calculator2.git" target="_blank">GitHub</a>
    </div>
  </div>

  <div class="card" data-aos="fade-up" data-aos-duration="1000">
    <img class="card-image" src="../assets/One-Piece-Store.png" alt="Card 3" />
    <div class="card-content">
      <h3 class="card-title">E-commerce site</h3>
      <p class="card-description">One Piece E-commerce</p>
      <a class="card-link" href="https://luntu-ecommerce.netlify.app/" target="_blank">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/e-commerce.git" target="_blank">GitHub</a>
    </div>
  </div>

  <div class="card" data-aos="fade-up" data-aos-duration="1000">
    <img class="card-image" src="https://i.postimg.cc/bN9Pf3cR/portfolio.png" alt="Card 4" />
    <div class="card-content">
      <h3 class="card-title">Bootstrap Portfolio</h3>
      <p class="card-description">My very first portfolio create using html, css, and boostrap</p>
      <a class="card-link" href="https://luntu-portfolio.netlify.app/" target="_blank">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/Portfolio.git" target="_blank">GitHub</a>
    </div>
  </div>

  <div class="card" data-aos="fade-up" data-aos-duration="1000">
    <img class="card-image" src="../assets/ArchievableGaming.gif" alt="Card 5" />
    <div class="card-content">
      <h3 class="card-title">Archie-Vable Gaming</h3>
      <p class="card-description">An e-commerce site for gamers looking for gaming components</p>
      <a class="card-link" href="https://archie-vable-gaming.web.app/" target="_blank">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/Archie-VableGaming.git" target="_blank">GitHub</a>
    </div>
  </div>

  <div class="card" data-aos="fade-up" data-aos-duration="1000">
    <img class="card-image" src="../assets/checklist-to-do.gif" alt="Card 6" />
    <div class="card-content">
      <h3 class="card-title">To-do List</h3>
      <p class="card-description">Created a checklist to help me remember my tasks</p>
      <a class="card-link" href="https://luntuchecklist.netlify.app/" target="_blank">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/luntuchecklist.git" target="_blank">GitHub</a>
  </div>
</div>

<div class="card" data-aos="fade-up" data-aos-duration="1000">
    <img class="card-image" src="../assets/One_Piece_Merch.png" alt="Card 8" />
    <div class="card-content">
      <h3 class="card-title">One Piece Merch</h3>
      <p class="card-description">My very first One Piece wordpress e-commerce site</p>
      <a class="card-link" href="https://dev-onepiecemerch.pantheonsite.io/" target="_blank">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/luntuchecklist.git" target="_blank">GitHub</a>
  </div>
</div>

<div class="card" data-aos="fade-up" data-aos-duration="1000">
    <img class="card-image" src="../assets/Katana-kingdom.png" alt="Card 7" />
    <div class="card-content">
      <h3 class="card-title">Wordpress</h3>
      <p class="card-description">A wordpress project I worked on with my fellow colleagues</p>
      <a class="card-link" href="https://dev-katana-kingdom.pantheonsite.io/" target="_blank">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/luntuchecklist.git" target="_blank">GitHub</a>
  </div>
</div>

<div class="card" data-aos="fade-up" data-aos-duration="1000">
    <img class="card-image" src="../assets/RPS.jpg" alt="Card 7" />
    <div class="card-content">
      <h3 class="card-title">RPS Game</h3>
      <p class="card-description">A Rock, Papers, Scissors game I developed using python code</p>
      <a class="card-link" href="http://luntu.pythonanywhere.com/" target="_blank">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/newrpsgame.git" target="_blank">GitHub</a>
  </div>
</div>

<div class="card" data-aos="fade-up" data-aos-duration="1000">
    <img class="card-image" src="../assets/NewProjectGif.gif" alt="Card 9" />
    <div class="card-content">
      <h3 class="card-title">Project in progress</h3>
      <p class="card-description">There's a project currently in progress. Please wait.</p>
      <a class="card-link" href="...">nothing</a>
      <a class="card-link" href="...">yet</a>
  </div>
</div>
</div>

</template>

<script>
export default {
  mounted() {
    AOS.init();
  }
}
</script>

<style scoped>
#projects {
  margin-top: 50px;
  overflow-y: hidden;
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

.card-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding-left: 80px; 
  padding-right: 80px; 
}

.card {
  width: 300px;
  margin-top: 28px;
  margin-bottom: 40px;
  color: yellow;
  background-color: rgb(62, 61, 61);
  border-radius: 10px;
  border: 2px solid yellow;

  /* box-shadow: 0px 5px 15px yellow; */
}

.card:hover {
  transition: 0.2s ease-in;
  transform: scale(1.1);
    box-shadow: 0px 0px 10px 3px yellow;

}

.card-image {
  width: 100%;
  height: 200px;
  object-fit: cover;
  object-position: center;
  border-radius: 9px 9px 0px 0px;
}

.card-content {
  padding: 20px;
}

.card-title {
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 10px;
}

.card-description {
  font-size: 16px;
  margin-bottom: 20px;
  color: white !important;
}

.card-link {
  width: 120px;
  height: 40px;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  font-size: 16px;
  font-weight: bold;
  text-transform: uppercase;
  cursor: pointer;
  transition: all 0.3s ease;
  background-color: black;
  color: yellow;
  text-align: center;
  line-height: 20px;
  margin-bottom: 10px;
  text-decoration: none;
}

.card-link:nth-of-type(1),
.card-link:nth-of-type(2) {
  background-color: black;
  color: yellow;
}

.card-link:hover {
  background-color: yellow;
  color: black;
}

@media screen and (max-width: 759px) {
  .card {
    width: calc(100% - 20px);
  }
}

@media screen and (max-width: 450px) {
  .card {
    width: calc(100% - 20px);
  }
}

</style>
