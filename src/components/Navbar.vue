<template>
  <nav>
    <div class="Logo">
      <a href="#">
        <img src="../assets/Temporary__logo-removebg-preview.png" style="height: 70px; width: auto;" alt="Logo">
      </a>
    </div>
    <input type="checkbox" id="menu-toggle" class="menu-toggle-input">
    <label class="menu-button-container" for="menu-toggle">
      <div class="menu-button"></div>
    </label>
    <ul class="menu">
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
  /* overflow-x: hidden; */
}

.menu > li {
  margin: 0 1rem;
}

.menu-button-container {
  display: none;
  height: 100%;
  width: 30px;
  cursor: pointer;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.menu-button {
  background-color: yellow;
}

.menu-toggle-input {
  display: none;
}

.menu-button,
.menu-button::before,
.menu-button::after {
  display: block;
  background-color: #fff;
  position: absolute;
  height: 4px;
  width: 30px;
  transition: transform 400ms cubic-bezier(0.23, 1, 0.32, 1);
  border-radius: 2px;
}

.menu-button::before {
  content: '';
  margin-top: -8px;
  background-color: yellow;
}

.menu-button::after {
  content: '';
  margin-top: 8px;
  background-color: yellow;
}

.menu-toggle-input:checked + .menu-button-container .menu-button::before {
  margin-top: 0px;
  transform: rotate(45deg);
}

.menu-toggle-input:checked + .menu-button-container .menu-button::after {
  margin-top: 0px;
  transform: rotate(-45deg);
}

.menu-toggle-input:checked + .menu-button-container .menu-button {
  background-color:  rgb(62, 61, 61);
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
  max-height: 0;
  overflow: hidden;
  transition: max-height 400ms cubic-bezier(0.23, 1, 0.32, 1);
}

.menu-toggle-input:checked + .menu-button-container + ul {
  max-height: 200px; 
}

li {
  margin-left: 1rem;
}

li:hover, li:focus {
  opacity: 0.5;
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

@media (max-width: 767.20px){
  .menu-button-container{
    display: flex;
  }

  .menu {
    position: absolute;
    top: 70px; 
    left: 0;
    flex-direction: column;
    width: 100%;
    background-color: rgb(62, 61, 61);
    transition: max-height 400ms cubic-bezier(0.23, 1, 0.32, 1);;
  }
  .menu-toggle-input:checked + .menu-button-container + ul {
    /* max-height: 200px; Adjust the max-height as needed for your content */
    max-height: none;

  }

  .menu > li {
    display: flex;
    justify-content: center;
    margin: 0;
    padding: 0.5em;
    width: 100%;
    color: white;
    background-color: #222;
    border-bottom: 1px solid #444;
  }


}

@media (min-width: 768px) {
  ul {
    padding: 0 100px;
    flex-wrap: nowrap; 
    justify-content: flex-start; 
    max-height: none;
    overflow: visible;
  }
}
</style>
