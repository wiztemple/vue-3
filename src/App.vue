<template>
  <HelloWorld msg="Welcome to Your Vue.js App" />
  <Basics />
  <Vmodel />
  <Vif />
  <Vbind />
  <Vfor />
  <Vonce />
  <Von />
  <Vtext />
  <DirectivesExercise />
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Basics from "./components/Basics";
import Vmodel from "./components/Vmodel";
import Vif from "./components/Vif";
import Vbind from "./components/Vbind";
import Vfor from "./components/Vfor";
import Vonce from "./components/Vonce";
import Von from "./components/Von";
import Vtext from "./components/Vtext";
import DirectivesExercise from "./components/DirectivesExercise";

export default {
  name: "App",
  components: {
    HelloWorld,
    Basics,
    Vmodel,
    Vif,
    Vbind,
    Vfor,
    Vonce,
    Von,
    Vtext,
    DirectivesExercise,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
