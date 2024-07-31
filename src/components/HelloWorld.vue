<template>
  <div class="frame-1">
    <div class="rectangle-1"></div>
    <img class="dsc-3496-removebg-2" src="../assets/ImageForPortfoliojpg-removebg-preview.png" />
    <div class="wrapper">
      <div class="hi-i-am-luntu-sogeyana">
        Hi, I am Luntu Sogeyana.
      </div>
      <p class="web-dev">
        I am a Web Developer
      </p>
      <div class="cv-button-container">
        <a target="_blank" href="https://drive.google.com/file/d/14jlJyfjEFYz4i6rMegl4EeMurUFmWkPe/view?usp=sharing" class="cv-button" download="Luntu_Sogeyana_CV">Download CV</a>
      </div>
    </div>
  </div>
</template>

<style scoped>
.frame-1 {
  width: 100%;
  max-width: 1500px;
  height: 673px;
  position: relative;
  overflow: hidden;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 20px;
}

.rectangle-1 {
  background: black;
  width: 100%;
  height: 100%;
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
}

.wrapper {
  max-width: 50%;
  text-align: left;
  position: relative;
}

.hi-i-am-luntu-sogeyana,
.web-dev {
  overflow: hidden; /* Ensures text doesn't overflow during animation */
  white-space: nowrap; /* Keeps text on one line */
  border-right: 0.15em solid yellow; /* Cursor */
  animation: typing 4s steps(40, end) forwards, blink-caret 0.75s step-end infinite;
}

.hi-i-am-luntu-sogeyana {
  color: yellow;
  font-weight: bold;
  font-size: 2.5rem;
  margin-bottom: 20px;
}

.web-dev {
  color: white;
  font-size: 1.5rem;
  margin-bottom: 20px;
  animation-delay: 4s; /* Delays the start of the web-dev typing animation */
  visibility: hidden;
}

.cv-button-container {
  margin-top: 20px;
}

.cv-button {
  display: inline-block;
  padding: 12px 24px;
  border: 2px solid yellow;
  background-color: black;
  color: yellow;
  font-size: 18px;
  text-decoration: none;
  border-radius: 4px;
  transition: all 0.2s ease-in-out;
}

.cv-button:hover {
  background-color: yellow;
  color: black;
}

.dsc-3496-removebg-2 {
  width: 45%;
  height: auto;
  margin-right: 20px;
}

@keyframes typing {
  from {
    width: 0;
    visibility: visible;
  }
  to {
    width: 100%;
    visibility: visible;
  }
}

@keyframes blink-caret {
  from, to {
    border-color: transparent;
  }
  20% {
    border-color: yellow;
  }
}

@keyframes blink-caret-stop {
  0%, 100% {
    border-color: transparent;
  }
}
</style>

.frame-1 {
  width: 100%;
  max-width: 1500px;
  height: 673px;
  position: relative;
  overflow: hidden;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 20px;
}

.rectangle-1 {
  background: black;
  width: 100%;
  height: 100%;
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
}

.wrapper {
  max-width: 50%;
  text-align: left;
  position: relative;
}

.hi-i-am-luntu-sogeyana,
.web-dev {
  overflow: hidden; /* Ensures text doesn't overflow during animation */
  white-space: nowrap; /* Keeps text on one line */
  border-right: 0.15em solid yellow; /* Cursor */
  animation: typing 4s steps(40, end) forwards, blink-caret 0.75s step-end infinite;
}

.hi-i-am-luntu-sogeyana {
  color: yellow;
  font-weight: bold;
  font-size: 2.5rem;
  margin-bottom: 20px;
}

.web-dev {
  color: white;
  font-size: 1.5rem;
  margin-bottom: 20px;
  animation-delay: 4s; /* Delays the start of the web-dev typing animation */
  animation: typing 4s steps(30, end) forwards, blink-caret-stop 8s steps(1, end) forwards;
  border-right: 0.15em solid white; /* Different color cursor */
  visibility: hidden; /* Initially hide the text */
}

.cv-button-container {
  margin-top: 20px;
}

.cv-button {
  display: inline-block;
  padding: 12px 24px;
  border: 2px solid yellow;
  background-color: black;
  color: yellow;
  font-size: 18px;
  text-decoration: none;
  border-radius: 4px;
  transition: all 0.2s ease-in-out;
}

.cv-button:hover {
  background-color: yellow;
  color: black;
}

.dsc-3496-removebg-2 {
  width: 45%;
  height: auto;
  margin-right: 20px;
}

@keyframes typing {
  from {
    width: 0;
    visibility: visible; /* Make text visible when typing starts */
  }
  to {
    width: 100%;
  }
}

@keyframes blink-caret {
  from, to {
    border-color: transparent;
  }
  50% {
    border-color: yellow;
  }
}

@keyframes blink-caret-stop {
  0%, 100% {
    border-color: transparent;
  }
}
