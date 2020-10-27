<template>
  <div class="vbind">
    <h3>V-For Example</h3>
    <p v-for="(value, key, index) in jokes" :key="value">
      {{ index }}. {{ key }}: {{ value }}
    </p>
  </div>
</template>

<script>
export default {
  name: "Vfor",
  data() {
    return {
      jokes: {
        question: "What did one baby prototype say to the other?",
        answer: `I'll race you to class!`,
        response: "groan",
      },
    };
  },
};
</script>

<style scoped>
</style>
