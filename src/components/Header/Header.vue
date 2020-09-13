<template>
  <div class="header-container">
    <video
      preload="auto"
      poster="../../assets/daniel-ricciardo.jpeg"
      src="../../assets/daniel-ricciardo-intro.mp4"
      autoplay
      loop
      playsinline
      video
    />
    <header class="viewport-header">
      <h1>
        {{ CONSTANTS.FIRST_NAME }}
        <span>{{ CONSTANTS.LAST_NAME }}</span>
      </h1>
    </header>
    <div class="content">
      <p>{{ CONSTANTS.CONTENT_ONE }}</p>
      <p>{{ CONSTANTS.CONTENT_TWO }}</p>
      <p>{{ CONSTANTS.CONTENT_THREE }}</p>
    </div>
  </div>
</template>

<script>
import constants from "../../config/constants";
export default {
  name: "Header",
  data() {
    return {
      CONSTANTS: constants,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
video {
  object-fit: cover;
  width: 100vw;
  height: 100vh;
  position: fixed;
  top: 0;
  left: 0;
}

.viewport-header {
  position: relative;
  height: 100vh;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
}

.content {
  background: rgba(black, 0.66);
  color: white;
  position: relative;
  padding: 4rem;
}

p {
  max-width: 80%;
  margin: 1rem auto;
  font-size: 2rem;
}

@media (max-width: 600px) {
  p {
    font-size: 1rem;
  }
}

h1 {
  font-family: "Syncopate", sans-serif;
  color: white;
  text-transform: uppercase;
  letter-spacing: 3vw;
  line-height: 1.2;
  font-size: 3vw;
  text-align: center;
}

span {
  display: block;
  font-size: 10vw;
  letter-spacing: -1.3vw;
}
</style>
