<template>
  <h1>Contact</h1>
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
  margin: 0 auto;
  margin-bottom: 50px;
  padding: 20px;
  color: yellow;
  border: 2px solid yellow;
  border-radius: 5px;
  height: 69vh;
  background-color: rgb(62, 61, 61);
  /* box-shadow: 0px 5px 15px yellow; */
  overflow-x: hidden;
  overflow-y: hidden;
  transition: 0.01s;
}

.contact:hover {
    box-shadow: 0px 5px 15px yellow;
}

button, input, optgroup, select, textarea {
  background-color: black;
  color: yellow;
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
  padding-bottom: 10px;
  margin-bottom: 10px;
  border-radius: 5px;
  /* box-shadow: 0px 5px 15px yellow; */
  font-size: 16px;
}

button[type="submit"] {
  display: block;
  margin: 0 auto;
  padding: 10px 20px;
  border-radius: 5px;
  border: 2px solid yellow;
  /* box-shadow: 0px 5px 15px yellow; */
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
</style>

