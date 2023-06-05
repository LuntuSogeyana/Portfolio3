<template>
  <nav>
    <div class="Logo">
      <a href="#">
        <img src="https://i.postimg.cc/KvLk1q53/new-logo-removebg-preview-1-removebg-preview.png" alt="Logo">
      </a>
    </div>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#testimonials">Testimonials</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</template>

<style scoped>
nav {
  position: sticky;
  top: 0;
  background-color: rgb(62, 61, 61);
  color: #fff;
  display: flex;
  justify-content: end;
  padding: 1rem;
  z-index: 1;
  height: 70px;
  border-bottom: 2px solid yellow;
  box-shadow: 0px 5px 15px yellow;
}

ul {
  display: flex;
  list-style: none;
  margin: 0;
  padding: 0;
  color: yellow;
  text-decoration: none;
  font-family: Arial, sans-serif;
  font-size: 20px;
}

li {
  margin-left: 1rem;
}

a {
  color: yellow;
  text-decoration: none;
  font-family: Arial, sans-serif;
}

.Logo {
  margin-right: auto;
  display: flex;
  align-items: center;
}

.Logo img { /* Adjust logo size later */
  width: 90px; 
  height: auto; 
}

@media (min-width: 768px) {
  ul {
    padding: 0 100px;
  }
}
</style>


  