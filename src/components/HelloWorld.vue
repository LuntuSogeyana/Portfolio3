<template>
  <div class="frame-1">
    <div class="rectangle-1"></div>
    <div class="rectangle-10"></div>
    <div class="hi-i-am-luntu-sogeyana-a-web-developer">
      Hi, I am  Luntu Sogeyana.
    </div>
    <p class="Web-dev">
      I am a Web Developer
    </p>
    <img class="dsc-3496-removebg-2" src="https://i.postimg.cc/Hxv8CVdV/DSC-3496-removebg.png" />
  </div>
</template>

<script>
export default {
  name: 'HelloWorld'
}
</script>

<style scoped>
.frame-1,
.frame-1 * {
  box-sizing: border-box;
  overflow-x: hidden;

}

.frame-1 {
  width: 100%;
  max-width: 1500px; /* Set the maximum width */
  height: 673px;
  position: relative;
  overflow: hidden;
  margin: 0 auto; /* Center the frame horizontally */
  overflow-x: hidden;
}

.rectangle-1 {
  background: black;
  width: 100%;
  max-width: 1520px; /* Set the maximum width */
  height: 673px;
  position: absolute;
  left: 50%;
  transform: translateX(-50%); /* Center the rectangle horizontally */
  top: 0px;
}

.navigation {
  position: absolute;
  inset: 0;
}

.about,
.projects,
.testimonials,
.contact-me,
.home {
  color: #000000;
  text-align: left;
  font: 400 20px "Inter", sans-serif;
  position: absolute;
  top: 43px;
}

.about {
  left: 1067px;
}

.projects {
  left: 1220px;
}

.testimonials {
  left: 1373px;
}

.contact-me {
  left: 1525px;
}

.home {
  left: 915px;
}

.hi-i-am-luntu-sogeyana-a-web-developer {
  color: yellow;
  text-align: left;
  /* font-family: 'Inter', sans-serif; */
  font-weight: bold;
  /* font-family: Arial, sans-serif;  */
  font-size: 70px;
  position: relative;
  left: 620px;
  top: 259px;
  width: 586px;
  width: max-content;

}

.Web-dev {
  color: yellow;
  text-align: left;
  /* font-family: Arial, sans-serif;  */
  font-weight: bold;
  /* font-family: 'Inter'; */
  font-size: 44px;
  position: relative;
  left: 620px;
  top: 259px;
  width: 586px;
  width: max-content;
}

.hi-i-am-luntu-sogeyana-a-web-developer::after,
.hi-i-am-luntu-sogeyana-a-web-developer::before {
  content: '';
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
}

.hi-i-am-luntu-sogeyana-a-web-developer::before {
  background-color: black;
  animation: typewriter 2s steps(24) forwards, blink;
}

.hi-i-am-luntu-sogeyana-a-web-developer::after {
  width: 0.125rem;
  background-color: yellow;
  animation: typewriter 2s steps(24) forwards, blink 500ms steps(24) infinite;
}

@keyframes typewriter {
  to {
    left: 100%;
  }
}

@keyframes blink {
  0% {
    visibility: hidden;
  }
  50% {
    visibility: hidden;
  }
  100% {
    visibility: visible;
  }
}

.dsc-3496-removebg-2 {
  width: 533px;
  height: 751px;
  position: absolute;
  left: 50px;
  top: -81px;
}

/* Mobile Responsive */

@media screen and (max-width: 768px) {
  .frame-1 {
    width: 100%;
    height: auto;
  }

  .rectangle-1 {
    width: 100%;
    height: auto;
  }

  .about,
  .projects,
  .testimonials,
  .contact-me,
  .home {
    font-size: 16px;
  }

  .hi-i-am-luntu-sogeyana-a-web-developer,
  .Web-dev {
    font-size: 28px;
    left: 50%;
    transform: translateX(-50%);
    width: 100%;
    text-align: center;
    top: 50%;
    max-width: 586px;
    margin-top: -14px;
  }

  .dsc-3496-removebg-2 {
    width: 100%;
    height: auto;
    position: relative;
    top: 0;
    left: 0;
    margin: 20px 0;
  }
}

</style>


