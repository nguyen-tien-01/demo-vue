<template>
  <CompHome />
</template>

<script>
import CompHome from "./components/CompHome.vue";

export default {
  name: "App",
  components: {
    CompHome,
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  /* font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px; */
  background-color: #D980FA;
  min-height: 620px;
  display: flex;
 
}
</style>
