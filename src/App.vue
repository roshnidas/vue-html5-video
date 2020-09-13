<template>
  <div id="app">
    <Tribute></Tribute>
  </div>
</template>

<script>
import Tribute from "./components/Tribute/Tribute";

export default {
  name: "App",
  components: {
    Tribute,
  },
};
</script>

<style>
body {
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
}
</style>
