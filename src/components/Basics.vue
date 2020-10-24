<template>
  <div class="basics">
    <ul>
      <li v-for="item in items" v-bind:key="item">
        {{ item }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Basics",
  data() {
    return {
      items: [
        "Sadio Mane",
        "Roberto Firmino",
        "Mohammed Salah",
        "Diogo Jota",
        "Thiago Alcantara",
        "Fabinho",
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
