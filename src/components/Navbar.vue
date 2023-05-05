<template>
    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Projects</a></li>
        <li><a href="#">Testimonials</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </template>
  
  <script>
  export default {
    name: 'Navbar'
  }
  </script>
  
  <style scoped>
  nav {
    background-color: rgb(62, 61, 61);
    color: #fff;
    display: flex;
    justify-content: end;
    padding: 1rem;
  }
  
  ul {
    display: flex;
    list-style: none;
    margin: 0;
    padding: 0 100px;
  }
  
  li {
    margin-left: 1rem;
  }
  
  a {
    color: yellow;
    text-decoration: none;
    font-family: 'Times New Roman', Times, serif;
  }
  </style>
  