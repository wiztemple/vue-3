<template>
  <div class="vonce">
    <h3>What is your favorite kind of taco?</h3>
    <p><input v-model="tacos" /></p>
    <p v-once>{{ tacos }}</p>
    <span v-pre
      >This is good if I need to show the mustache view of {{ tacos }}</span
    >
    <pre>{{ $data }}</pre>
  </div>
</template>

<script>
// V-Once / V_pre
// Not quite as useful, v-once will not update once it's been rendered
//v-pre will print out the inner text exactly how it is,including code(good for documentation)
export default {
  name: "Vonce",
  data() {
    return {
      tacos: "I like Al Pastor tacos",
    };
  },
};
</script>
<style scoped>
</style>
