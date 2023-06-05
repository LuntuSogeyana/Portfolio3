<template>
  <footer class="footer-clean">
    <div class="container">
      <div class="footer-row">
        <div class="footer-col">
          <h3>About Us</h3>
          <ul>
            <li><a href="#">Company</a></li>
            <li><a href="#">Team</a></li>
            <li><a href="#">Careers</a></li>
          </ul>
        </div>
        <div class="footer-col">
          <h3>Services</h3>
          <ul>
            <li><a href="#">Web Design</a></li>
            <li><a href="#">Development</a></li>
            <li><a href="#">Marketing</a></li>
          </ul>
        </div>
        <div class="footer-col">
          <h3>Contact Details</h3>
          <ul>
            <li><a>Email:<br>sogeyanaluntu@gmail.com</a></li>
            <li><a>Phone:<br>+27 67 826 7299</a></li>
            <li><a>Address:<br>sogeyanaluntu@gmail.com</a></li>
          </ul>
        </div>
      </div>
      <div class="footer-row">
        <div class="footer-col footer-social">
          <h3>Follow Me</h3>
          <a href="#"><i class="fab fa-facebook-f"></i></a>
          <a href="#"><i class="fab fa-twitter"></i></a>
          <a href="#"><i class="fab fa-instagram"></i></a>
        </div>
      </div>
      <div class="footer-row">
        <div class="footer-col text-center">
          <p class="mt-4 mb-0">
            &copy; 2023 Luntu Sogeyana Portfolio. All rights reserved.
          </p>
        </div>
      </div>
    </div>
  </footer>
</template>

  
  <script>
  export default {
    name: 'Footer'
  }
  </script>
  
  <style scoped>
.footer-clean {
  padding: 50px 0;
  background-color: rgb(62, 61, 61);
  color: yellow;
}

.footer-clean h3 {
  margin-top: 0;
  margin-bottom: 12px;
  font-weight: bold;
  font-size: 16px;
}

.footer-clean ul {
  padding: 0;
  list-style: none;
  line-height: 1.6;
  font-size: 14px;
  margin-bottom: 0;
}

.footer-clean ul a {
  color: inherit;
  text-decoration: none;
  opacity: 0.8;
}

.footer-clean ul a:hover {
  opacity: 1;
}

.footer-clean .footer-row {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.footer-clean .footer-col {
  flex-basis: 25%;
  text-align: center;
}

.footer-clean .footer-social {
  flex-basis: 100%;
}

.footer-clean .footer-social a {
  display: inline-block;
  width: 40px;
  height: 40px;
  line-height: 40px;
  text-align: center;
  border-radius: 50%;
  border: 1px solid yellow;
  margin: 0 5px;
  font-size: 24px;
  opacity: 0.75;
}

.footer-clean .footer-social a:hover {
  opacity: 0.9;
}

.footer-clean .text-center {
  text-align: center;
}

.footer-clean p {
  margin-top: 14px;
  margin-bottom: 0;
  font-size: 13px;
  opacity: 0.6;
}
</style>

  