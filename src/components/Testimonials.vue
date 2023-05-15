<template>
  <div class="content-wrapper">
    <h1>Testimonials</h1>
    <div class="blue-line"></div>
    <div class="wrapper-for-arrows">
      <div class="arrow-wrap left-arrow-wrap" @click="prevTestimonial">
        <div class="arrow"></div>
      </div>
      <div class="review-wrap">
        <div id="imgDiv">
          <img :src="testimonial.image" :alt="testimonial.name" />
        </div>
        <div id="personName">{{ testimonial.name }}</div>
        <div id="profession">{{ testimonial.profession }}</div>
        <div id="description">{{ testimonial.description }}</div>
      </div>
      <div class="arrow-wrap right-arrow-wrap" @click="nextTestimonial">
        <div class="arrow"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      testimonials: [
        {
          name: "Joel M.",
          profession: "Lecturer",
          description:
            "Vivamus condimentum sagittis magna non facilisis. Nullam vestibulum odio quis nunc lobortis, id laoreet justo scelerisque. Mauris faucibus ultricies felis vitae sagittis.",
          image: "https://i.postimg.cc/Ghbvn8KL/Joel-Profile.jpg"
        },
        {
          name: "Sakhe",
          profession: "Web Developer",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed vitae mi ut massa pellentesque lacinia. Curabitur dapibus tortor ut metus congue, sit amet finibus felis hendrerit.",
          image: "https://i.postimg.cc/Kz8bHftL/Sakhe.jpg"
        },
        {
          name: "Timmothy J.",
          profession: "Web Developer Intern",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed vitae mi ut massa pellentesque lacinia. Curabitur dapibus tortor ut metus congue, sit amet finibus felis hendrerit.",
          image: "https://i.postimg.cc/vH76FhmR/C11-1.jpg"
        },
        {
          name: "Brandon S.",
          profession: "Web Developer Intern",
          description:
            "Vivamus condimentum sagittis magna non facilisis. Nullam vestibulum odio quis nunc lobortis, id laoreet justo scelerisque. Mauris faucibus ultricies felis vitae sagittis.",
          image: "https://i.postimg.cc/QdGJWsyD/C11-Brandon-Swinton-1.jpg"
        },
        {
          name: "Konke M.",
          profession: "Web Developer Intern",
          description:
            "Vivamus condimentum sagittis magna non facilisis. Nullam vestibulum odio quis nunc lobortis, id laoreet justo scelerisque. Mauris faucibus ultricies felis vitae sagittis.",
          image: "https://i.postimg.cc/YCkHtYb1/DSC-3528.jpg"
        },
      ],
      currentTestimonialIndex: 0
    };
  },
  computed: {
    testimonial() {
      return this.testimonials[this.currentTestimonialIndex];
    }
  },
  methods: {
    prevTestimonial() {
      this.currentTestimonialIndex =
        (this.currentTestimonialIndex - 1 + this.testimonials.length) %
        this.testimonials.length;
    },
    nextTestimonial() {
      this.currentTestimonialIndex =
        (this.currentTestimonialIndex + 1) % this.testimonials.length;
    }
  }
};
</script>


<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Shippori+Antique&display=swap");

* {
	margin: 0;
	padding: 0;
	box-sizing: border-box;
}

button,
input,
select {
	font-family: inherit;
	font-size: 100%;
	box-sizing: border-box;
	padding: 0;
	margin: 0;
}

html {
	font-size: 12px;
}

body {
	color: #000;
	font-family: "Shippori Antique", sans-serif;
	height: 100vh;
	display: grid;
	place-items: center;
}

.content-wrapper {
	height: 100%;
	width: 70%;
	max-width: 100rem;
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	padding-bottom: 5rem;
  margin-left: 230px;
}

h1 {
	margin-bottom: calc(0.7rem + 0.5vmin);
	font-size: calc(2.3rem + 1vmin);
}

.blue-line {
	height: 0.3rem;
	width: 6rem;
	background-color: yellow;
	margin-bottom: calc(3rem + 2vmin);
}

.wrapper-for-arrows {
	position: relative;
	width: 70%;
	border-radius: 2rem;
	box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;
	overflow: hidden;
	display: grid;
	place-items: center;
}

.review-wrap {
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	padding-top: calc(2rem + 1vmin);
	width: 100%;
  background-color: grey;
  margin-left: 0px;
}

#imgDiv {
  border-radius: 50%;
  width: calc(6rem + 4vmin);
  height: calc(6rem + 4vmin);
  position: relative;
  box-shadow: 5px -3px yellow;
  background-size: cover;
  margin-bottom: calc(0.7rem + 0.5vmin);
  overflow: hidden;
}

#imgDiv {
    -webkit-animation: mover 1s infinite  alternate;
    animation: mover 1s infinite  alternate;
}
#imgDiv {
    -webkit-animation: mover 1s infinite  alternate;
    animation: mover 1s infinite  alternate;
}
@-webkit-keyframes mover {
    0% { transform: translateY(0); }
    100% { transform: translateY(-10px); }
}
@keyframes mover {
    0% { transform: translateY(0); }
    100% { transform: translateY(-10px); }
}

#imgDiv img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}


#imgDiv::after {
	content: "''";
	font-size: calc(2rem + 2vmin);
	font-family: sans-serif;
	line-height: 150%;
	color: #fff;
	display: grid;
	place-items: center;
	border-radius: 50%;
	background-color: yellow;
	position: absolute;
	top: 10%;
	left: -10%;
	width: calc(2rem + 2vmin);
	height: calc(2rem + 2vmin);
}

#personName {
	margin-bottom: calc(0.7rem + 0.5vmin);
	font-size: calc(1rem + 0.5vmin);
	letter-spacing: calc(0.1rem + 0.1vmin);
	font-weight: bold;
}

#profession {
	font-size: calc(0.8rem + 0.3vmin);
	margin-bottom: calc(0.7rem + 0.5vmin);
	color: yellow;
}

#description {
	font-size: calc(0.8rem + 0.3vmin);
	width: 70%;
	max-width: 40rem;
	text-align: center;
	margin-bottom: calc(1.4rem + 1vmin);
	color: rgb(92, 92, 92);
	line-height: 2rem;
}

.arrow-wrap {
	position: absolute;
	top: 50%;
}

.arrow {
	width: calc(1.4rem + 0.6vmin);
	height: calc(1.4rem + 0.6vmin);
	border: solid yellow;
	border-width: 0 calc(0.5rem + 0.2vmin) calc(0.5rem + 0.2vmin) 0;
	cursor: pointer;
	transition: transform 0.3s;
}

.arrow:hover {
	transition: 0.3s;
	transform: scale(1.15);
}

.left-arrow-wrap {
	left: 5%;
	transform: rotate(135deg);
	-webkit-transform: rotate(135deg);
  box-shadow: 0px 5px 15px yellow;
}

.right-arrow-wrap {
	transform: rotate(-45deg);
	-webkit-transform: rotate(-45deg);
	right: 5%;
  box-shadow: 0px 5px 15px yellow;
}

.move-head {
	animation: moveHead 1.55s infinite;
	animation-delay: -0.8s;
}

@keyframes moveHead {
	0% {
	}
	25% {
		transform: translate(0.5rem, 1rem) rotate(5deg);
	}
	100% {
		transform: translate(0, 0) rotate(-5deg);
	}
}

@media screen and (max-width: 900px) {
	.content-wrapper {
		width: 100%;
	}
}
</style>







  
  
  