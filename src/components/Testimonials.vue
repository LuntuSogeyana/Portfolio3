<template>
  <div id="testimonials" class="testimonials" v-intersect="onIntersect">
    <h2 class="testimonials__title">Testimonials</h2>
    <transition-group name="fade" tag="div" class="testimonials__list">
      <div class="testimonial" v-for="(testimonial, index) in testimonials" :key="index">
        <div class="testimonial__image" :style="{ 'animation-delay': `${index * 0.2}s` }">
          <img :src="testimonial.image" alt="testimonial author">
        </div>
        <div class="testimonial__text">{{ testimonial.text }}</div>
        <div class="testimonial__author">{{ testimonial.author }}</div>
      </div>
    </transition-group>
  </div>
</template>

<script>
export default {
  data() {
    return {
      testimonials: [
        {
          text: "Luntu is one of a kind, he has ideas you would think are impossible, until he shows you in the idea in it's fullest and you realize, he's a genius.He has a bright future in front of him and he's always willing to learn new types of things to broaden up he's knowledge.",
          author: 'Konke Malindi',
          image: 'https://via.placeholder.com/150'
        },
        {
          text: "Luntu is one of the most honest people you can come across. Very wise beyond his years with bright ideas which could shake the world in a very positive way. A man who is not afraid to live and speak his truth.",
          author: 'Sakhe Mzolisa',
          image: 'https://via.placeholder.com/150'
        },
        {
          text: "Luntu is a very creative, and well-behaved student. He does enjoy working with his classmates and works well on his project. He has gained knowledge of web development, including Bootstrap 5. I will be very delighted to see him get hired as a developer.",
          author: 'Joel Mukanya',
          image: 'https://i.postimg.cc/13xJQg6X/image.jpg'
        },
        {
          text: "Luntu is a hard-working guy who can accomplish anything he puts his mind to. He has a very friendly personality which makes it very easy to oproach him. He is very dedicated and committed to any project that he has set for himself.",
          author: 'Timothy Jennike',
          image: 'https://via.placeholder.com/150'
        },
        {
          text: "Luntu is a serious & fun individual who enjoys learning and exploring different things. He enthusiasm into his work allows him to be creative with the littlest of things, and never seems to fail to make the environment quite lively. You won't regret having him as part of your team.",
          author: 'Athenkosi Freddie',
          image: 'https://i.postimg.cc/YSgSPCg1/IMG-20221004-074457-848.jpg'
        },
        {
          text: 'Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus.',
          author: 'Emma Johnson',
          image: 'https://via.placeholder.com/150'
        }
      ],
      animate: false
    }
  },
  methods: {
    onIntersect(entries) {
      entries.forEach(entry => {
        this.animate = entry.isIntersecting
      })
    }
  }
}
</script>
  
<style scoped>
.testimonial-image {
  opacity: 0;
  animation: fade-in 0.5s ease-in-out forwards;
}

@keyframes fade-in {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.testimonials {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
}

.testimonial-list {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}

.testimonial {
  width: calc(33.33% - 10px);
  margin-bottom: 20px;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 5px;
  box-sizing: border-box;
}

.testimonial-image {
  margin-bottom: 20px;
}

.testimonial-image img {
  display: block;
  max-width: 100%;
  height: auto;
  border-radius: 50%;
}

.testimonial-text {
  margin-bottom: 10px;
  color: yellow;
}

.testimonial-author {
  font-weight: bold;
  color: yellow;
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s;
}

.fade-enter,
.fade-leave-to {
  opacity: 0;
}

@media (max-width: 800px) {
  .testimonial {
    width: calc(50% - 10px);
  }
}

@media (max-width: 600px) {
  .testimonial {
    width: 100%;
  }
}
</style>


  
  
  