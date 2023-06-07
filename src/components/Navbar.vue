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

<script>

</script>

<style scoped>
nav {
  position: sticky;
  top: 0;
  background-color: rgb(62, 61, 61);
  color: #fff;
  display: flex;
  justify-content: flex-end;
  padding: 1rem;
  z-index: 1;
  height: 70px;
  border-bottom: 2px solid yellow;
  overflow-x: hidden;
}

ul {
  display: flex;
  list-style: none;
  margin: 0;
  padding: 0;
  color: yellow;
  text-decoration: none;
  font-size: 20px;
  flex-wrap: wrap;
  justify-content: flex-end; 
}

li {
  margin-left: 1rem;
}

li :hover,li:focus {
  opacity: 50%;
}

a {
  color: yellow;
  text-decoration: none;
}

.Logo {
  margin-right: auto;
  display: flex;
  align-items: center;
}

.Logo img { 
  width: 90px; 
  height: auto; 
}

@media (min-width: 768px) {
  ul {
    padding: 0 100px;
    flex-wrap: nowrap; 
    justify-content: flex-start; 
  }
}
</style>


  