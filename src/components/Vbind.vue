<template>
  <div class="vbind">
    <h3>Who is your favorite boxer?</h3>
    <textarea v-model="flyod" />
    <br />
    <button :class="[flyod ? activeClass : '']">Let us know</button>
  </div>
</template>

<script>
// V-Bind or :
// One of the most useful directives, so there's a shortcut
// We can use it for so many things: class and style binding, creating dynamic props
export default {
  name: "Vbind",
  data() {
    return {
      flyod: "",
      activeClass: "active",
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
button {
  padding: 10px 30px;
  border: none;
  border-radius: 5px;
}
button.active {
  background-color: orangered;
  color: #fff;
}
</style>
