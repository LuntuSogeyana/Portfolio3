<template>
<div class="card-container">

  <div class="card">
    <img class="card-image" src="https://i.postimg.cc/YqFYCBDH/Luffy-Flip-card-final.png" alt="Card 2" />
    <div class="card-content">
      <h3 class="card-title">Flip-card</h3>
      <p class="card-description">A flip card of Monkey D. Luffy</p>
      <a class="card-link" href="">Demo</a>
      <a class="card-link" href="">GitHub</a>
     </div>
  </div>

  <div class="card">
    <img class="card-image" src="https://i.postimg.cc/gcZ67Tnz/Calculator.jpg" alt="Card 1" />
    <div class="card-content">
      <h3 class="card-title">Calculator</h3>
      <p class="card-description">Description of project 1.</p>
      <a class="card-link" href="https://luntucalculator.netlify.app/">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/Calculator2.git">GitHub</a>
    </div>
  </div>

  <div class="card">
    <img class="card-image" src="https://i.postimg.cc/t46WSGGT/Screenshot-2022-11-01-090450.png" alt="Card 3" />
    <div class="card-content">
      <h3 class="card-title">E-commerce site</h3>
      <p class="card-description">An e-commerce site that sells One Piece merchandise.</p>
      <a class="card-link" href="https://luntu-ecommerce.netlify.app/">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/e-commerce.git">GitHub</a>
    </div>
  </div>

  <div class="card">
    <img class="card-image" src="https://i.postimg.cc/bN9Pf3cR/portfolio.png" alt="Card 4" />
    <div class="card-content">
      <h3 class="card-title">Bootstrap Portfolio</h3>
      <p class="card-description">Description of project 4.</p>
      <a class="card-link" href="https://luntu-portfolio.netlify.app/">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/Portfolio.git">GitHub</a>
    </div>
  </div>

  <div class="card">
    <img class="card-image" src="https://i.postimg.cc/bvdB7nFH/Archie-Vable-Gaming.png" alt="Card 5" />
    <div class="card-content">
      <h3 class="card-title">Capstone Project</h3>
      <p class="card-description">Description of project 5.</p>
      <a class="card-link" href="https://archie-vable-gaming.web.app/">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/Archie-VableGaming.git">GitHub</a>
    </div>
  </div>

  <div class="card">
    <img class="card-image" src="https://i.postimg.cc/cLPDJt3L/To-do-list.png" alt="Card 6" />
    <div class="card-content">
      <h3 class="card-title">To-do List</h3>
      <p class="card-description">Created a checklist to help me remember my tasks</p>
      <a class="card-link" href="https://luntuchecklist.netlify.app/">Demo</a>
      <a class="card-link" href="https://github.com/ManakiX/luntuchecklist.git">GitHub</a>
  </div>
</div>

</div>

</template>

<style>
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

  background-color: white;
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
