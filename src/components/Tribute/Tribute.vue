<template>
  <div class="tribute-div">
    <div class="image-container">
      <Header></Header>
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
import Footer from "../Footer/Footer";
import Header from "../Header/Header";

export default {
  name: "Tribute",
  components: {
    Footer,
    Header,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.image-container {
  display: flex;
  justify-content: center;
}
</style>
