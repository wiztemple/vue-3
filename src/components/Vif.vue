<template>
  <div class="vif">
    <h3>Who is your favorite player?</h3>
    <textarea v-model="messi" />
    <br />
    <button v-if="messi" type="submit">Let us know</button>
    <button v-show="messi" type="submit">Ah Messi Again</button>
    <input v-model="messi" type="radio" value="yes" id="yes" />
    <label for="yes">Yes</label><br />
    <input v-model="messi" type="radio" value="no" id="yes" />
    <label for="no">No</label><br />
    <p v-if="messi === 'yes'">Cool!</p>
    <p v-else-if="messi === 'no'">Damn!</p>
  </div>
</template>

<script>
// V-If / V-Show
// Is a conditional that will display information depending on meeting a requirement. this can be anything - buttons, forms, divs, components
// v-show hides the element, adds display: none
export default {
  name: "Vif",
  data() {
    return {
      messi: "",
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
