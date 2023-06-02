<template>
<div id="projects" class="card-container">

  <div class="card">
    <img class="card-image" src="https://i.postimg.cc/YqFYCBDH/Luffy-Flip-card-final.png" alt="Card 2" />
    <div class="card-content">
      <h3 class="card-title">Flip-card</h3>
      <p class="card-description">A flip card of Monkey D. Luffy</p>
      <a class="card-link" href="https://silver-eclair-a67fc6.netlify.app/" target="_blank">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/flip--card.git" target="_blank">GitHub</a>
     </div>
  </div>

  <div class="card">
    <img class="card-image" src="https://i.postimg.cc/gcZ67Tnz/Calculator.jpg" alt="Card 1" />
    <div class="card-content">
      <h3 class="card-title">Calculator</h3>
      <p class="card-description">A simple calculator .</p>
      <a class="card-link" href="https://luntucalculator.netlify.app/" target="_blank">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/Calculator2.git" target="_blank">GitHub</a>
    </div>
  </div>

  <div class="card">
    <img class="card-image" src="https://i.postimg.cc/t46WSGGT/Screenshot-2022-11-01-090450.png" alt="Card 3" />
    <div class="card-content">
      <h3 class="card-title">E-commerce site</h3>
      <p class="card-description">One Piece E-commerce</p>
      <a class="card-link" href="https://luntu-ecommerce.netlify.app/" target="_blank">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/e-commerce.git" target="_blank">GitHub</a>
    </div>
  </div>

  <div class="card">
    <img class="card-image" src="https://i.postimg.cc/bN9Pf3cR/portfolio.png" alt="Card 4" />
    <div class="card-content">
      <h3 class="card-title">Bootstrap Portfolio</h3>
      <p class="card-description">My very first portfolio create using html, css, and boostrap</p>
      <a class="card-link" href="https://luntu-portfolio.netlify.app/" target="_blank">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/Portfolio.git" target="_blank">GitHub</a>
    </div>
  </div>

  <div class="card">
    <img class="card-image" src="https://i.postimg.cc/bvdB7nFH/Archie-Vable-Gaming.png" alt="Card 5" />
    <div class="card-content">
      <h3 class="card-title">Archie-Vable Gaming</h3>
      <p class="card-description">E-commerce site for gamers on a budget</p>
      <a class="card-link" href="https://archie-vable-gaming.web.app/" target="_blank">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/Archie-VableGaming.git" target="_blank">GitHub</a>
    </div>
  </div>

  <div class="card">
    <img class="card-image" src="https://i.postimg.cc/cLPDJt3L/To-do-list.png" alt="Card 6" />
    <div class="card-content">
      <h3 class="card-title">To-do List</h3>
      <p class="card-description">Created a checklist to help me remember my tasks</p>
      <a class="card-link" href="https://luntuchecklist.netlify.app/" target="_blank">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/luntuchecklist.git" target="_blank">GitHub</a>
  </div>
</div>

</div>

</template>

<style>
#projects {
  margin-top: 50px;
}
  .card-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}

.card {
  width: calc(20.33% - 10px);
  margin-bottom: 0px;
  margin-top: 20px;
  margin-left: 70px;
  margin-right: 50px;
  font-family: Arial, sans-serif; 
  color: black;
  background-color: rgb(62, 61, 61);
  border-radius: 10px;
  box-shadow: 0px 5px 15px yellow;
  overflow: hidden;
}

.card-image {
  width: 100%;
  height: 200px;
  object-fit: cover;
  object-position: center;
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
}

.card-link:nth-of-type(1) {
  background-color: black;
  color: yellow;
}


.card-link:nth-of-type(2) {
  background-color: black;
  color: yellow;
}




.card-link:hover {
  background-color: yellow;
  color: black;
}

</style>
