<template>
  <div class="vtext">
    <h3>What is your favorite taco?</h3>
    <p v-html="tacos"></p>

    <h1>V-TEXT</h1>
    <h4>What is your favorite Migos singer?</h4>
    <p v-text="migos"></p>
    <p>{{ migos }}</p>
    <p>
      <input v-model="migos" />
    </p>
  </div>
</template>

<script>
// V-HTML or @
// Great for strings that have HTML elements that need to be rendered
// warning
// Not the same as templates: inserted as plain HTML. Don't use on user rendered content
// avoid XSS attacks
//V-TEXT
// similar to using template mustache
// Warning!
// If you want to dynamically update, it's recommneded to use template mustache instead

export default {
  name: "Vtext",
  data() {
    return {
      tacos: `I like <a href="www.google.com" target="_blank">Google</a>`,
      migos: "I Love Takeoff",
    };
  },
};
</script>
<style scoped>
</style>
