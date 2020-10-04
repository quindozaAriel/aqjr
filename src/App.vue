<template>
  <div id="app">
    <NavBar/>
    <LandingPage />
    <LandingPage />
  </div>
</template>

<script>
import LandingPage from "./components/LandingPage.vue";
import NavBar from "./components/NavBar.vue";

export default {
  name: "App",
  components: {
    LandingPage,
    NavBar
  },
};
</script>

<style lang="scss">
* {
  box-sizing: border-box;
  margin: 0;
  font-family: "Raleway", sans-serif;
  
}
/* width */
::-webkit-scrollbar {
  width: 8px;
  transition:1s;
}

/* Track */
::-webkit-scrollbar-track {
  background: #f1f1f1; 
}
 
/* Handle */
::-webkit-scrollbar-thumb {
  background: #888; 
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: #555; 
}
</style>