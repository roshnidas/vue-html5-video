<template>
  <div>
    <footer class="site-footer">
      <span class="site-footer-text">{{ CONSTANTS.FOOTER_TEXT }}</span>
    </footer>
  </div>
</template>

<script>
import constants from "../../config/constants";
export default {
  name: "Footer",
  data() {
    return {
      CONSTANTS: constants,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.site-footer {
  height: 64px;
  background: black;
  position: fixed;
  width: 100%;
  bottom: 0;
  justify-content: center;
  display: flex;
  align-items: center;
  color: white;
  font-size: 1rem;
}
</style>
