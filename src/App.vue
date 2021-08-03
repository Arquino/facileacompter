<template>
<!-- https://www.figma.com/file/GJRkoBvPmXNSS63o9bYMTn/FIDUCIE%2FFACILE-A-SIMULER?node-id=0%3A2 -->
  <header>
    <Navbar />
  </header>

    <Home />

  <footer></footer>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import Navbar from "./components/Navbar.vue";
import Home from "./pages/Home.vue";

export default {
  name: "App",
  components: {
    Navbar,
    Home,
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100&display=swap');
 @import url("https://fonts.googleapis.com/css2?family=Inter:wght@600&display=swap");
 @import url('https://fonts.googleapis.com/css2?family=Inter&display=swap');
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: inter;
}

header {
  width: 100%;
  height: 90px;
  justify-content: space-between;
  background-color: #fff;
  padding: 25px;
  display: flex;
  align-items: center;
  padding-left: 90px;
  padding-right: 90px;
}
body {
  background-color: #fef4ed;
  /* text-align: center; */
}
.bg {
  width: 100%;
  height: 500px;
  left: 0px;
  border-radius: 0px;
}
</style>
