<template>
  <div class="vmodel">
    <h3>Type Here</h3>
    <textarea v-model="message" class="message" rows="5" maxlength="72" />
    <br />
    <p class="booktext">{{ message }}</p>
    <input
      v-model="checkedNames"
      type="checkbox"
      id="sullivan"
      value="sullivan"
    />
    <label for="sullivan">Sullivan</label>
    <input v-model="checkedNames" type="checkbox" id="faith" value="faith" />
    <label for="faith">Faith</label>
    <input v-model="checkedNames" type="checkbox" id="ada" value="ada" />
    <label for="ada">Ada</label>
    <div>checkedNames: {{ checkedNames }}</div>

    <p>Another Example</p>
    <span v-for="option in options" :key="option">
      <input
        v-model="checkedNames"
        :id="option.value"
        value="option.value"
        type="checkbox"
      />
      <label for="option.value">{{ option.value }}</label>
    </span>
    <span>checked names: {{ checkedNames }} </span>
  </div>
</template>

<script>
// V-Model
// creates a relationship between the data in the instances/component and a fom input, so you can dynamically update values
export default {
  name: "Vmodel",
  data() {
    return {
      message: "This isa good place to type things",
      checkedNames: [],
      options: [
        { value: "Chinyere" },
        { value: "Brendan" },
        { value: "Edwin" },
        { value: "Felicia" },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
