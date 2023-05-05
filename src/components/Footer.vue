<template>
    <footer>
      <div class="social-icons">
        <a href="#" target="_blank"><i class="fab fa-linkedin"></i></a>
        <a href="#" target="_blank"><i class="fab fa-facebook"></i></a>
        <a href="#" target="_blank"><i class="fab fa-twitter"></i></a>
        <a href="#" target="_blank"><i class="fab fa-github"></i></a>
      </div>
      <p>&copy; 2023 Your Company. All Rights Reserved.</p>
    </footer>
  </template>
  
  <script>
  export default {
    name: 'Footer'
  }
  </script>
  
  <style scoped>
  footer {
    background-color: rgb(62, 61, 61);
    color: yellow;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 1rem;
  }
  
  .social-icons {
    display: flex;
    justify-content: center;
  }
  
  .social-icons a {
    margin-right: 1rem;
  }
  
  p {
    margin-top: 1rem;
    font-size: 0.8rem;
  }
  </style>
  