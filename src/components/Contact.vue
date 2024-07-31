<template>
  <h1 class="con-head">Contact</h1>
  <div class="blue-line"></div>
  <div id="contact" class="contact" data-aos="fade-up" data-aos-duration="1000">
    <h1>Contact Me</h1>
    <form action="https://formspree.io/f/mqkjbnav" method="POST">
      <div class="form-group">
        <label for="name">Name:</label>
        <input type="text" id="name" v-model="name" name="name" required>
      </div>
      <div class="form-group">
        <label for="email">Email:</label>
        <input type="email" id="email" v-model="email" name="email" required>
      </div>
      <div class="form-group">
        <label for="message">Message:</label>
        <textarea id="message" v-model="message" name="message" required></textarea>
      </div>
      <button type="submit">Submit</button>
    </form>
  </div>
</template>

<script scoped>
export default {
  name: 'Contact',
  mounted() {
    AOS.init();
  },
  data() {
    return {
      name: '',
      email: '',
      message: ''
    }
  },
  methods: {
    submitForm() {
     console.log('Form submitted!');
    }
  }
}
</script>

<style scoped>
#contact {
  margin-top: 50px;
}

.blue-line {
  height: 0.3rem;
  width: 6rem;
  background-color: yellow;
  margin-bottom: calc(3rem + 2vmin);
  margin-left: auto;
  margin-right: auto;
}

.contact {
  max-width: 600px;
  width: 90%;
  margin: 0 auto;
  margin-bottom: 50px;
  padding: 20px;
  color: white;
  border: 2px solid yellow;
  border-radius: 5px;
  min-height: 69vh;
  background-color: rgb(62, 61, 61);
  overflow: hidden;
  transition: box-shadow 0.3s ease-in-out;
}

.con-head {
  color: white;
  text-align: center;
  font-size: 2.5rem;
  margin-bottom: 1rem;
}

h1 {
  color: yellow;
  text-align: center;
  margin-bottom: 1.5rem;
}

.contact:hover {
  box-shadow: 0px 5px 15px yellow;
}

button,
input,
optgroup,
select,
textarea {
  background-color: black;
  color: yellow;
  border: 2px solid yellow;
  border-radius: 5px;
}

.form-group {
  margin-bottom: 20px;
}

label {
  display: block;
  margin-bottom: 5px;
  font-weight: bold;
}

input,
textarea {
  width: 100%;
  padding: 10px;
  border: none;
  border-radius: 5px;
  font-size: 16px;
  outline: none;
  transition: background-color 0.3s ease;
}

input:focus,
textarea:focus {
  background-color: #222;
}

button[type="submit"] {
  display: block;
  margin: 20px auto;
  padding: 10px 20px;
  border-radius: 5px;
  background-color: black;
  color: yellow;
  font-size: 16px;
  cursor: pointer;
  transition: all 0.2s ease-in-out;
}

button[type="submit"]:hover {
  background-color: yellow;
  color: black;
  font-weight: bold;
}

@media screen and (max-width: 600px) {
  .contact {
    padding: 15px;
  }

  .con-head {
    font-size: 2rem;
  }

  h1 {
    font-size: 1.5rem;
  }

  button[type="submit"] {
    padding: 8px 16px;
    font-size: 14px;
  }
}

</style>

