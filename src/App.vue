<template>
  <div id="app">
    <Exam/>
  </div>
</template>

<script>
import Exam from "./components/Exam";

export default {
  name: "App",
  components: {
    Exam
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
