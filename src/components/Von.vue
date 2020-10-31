<template>
  <div class="von">
    <div class="item">
      <img
        src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/28963/backpack.jpg"
        width="235"
        height="300"
      />
      <div class="quantity">
        <button class="inc" @click="counter > 0 ? (counter -= 1) : 0">-</button>
        <span class="quant-text">Quantity: {{ counter }}</span>
        <button class="inc" @click="counter += 1">+</button>
      </div>

      <button class="submit" @click="stop">Submit</button>
    </div>
    <!--item-->
  </div>
</template>

<script>
// V-On or @
// Extremely useful so there's a shortcut! v-on is great for binding to events like click and mouseenter.
// You're able to pass in a parameter for the event like (e)
// We can also use ternaries directly

export default {
  name: "Von",
  data() {
    return {
      counter: 0,
    };
  },
};
</script>
<style scoped>
.special {
  font-family: "Montserrat", sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  font-size: 12px;
}

li {
  list-style: none;
  display: inline-block;
}

input {
  background: #eee;
}

button {
  border: none;
  border-radius: 1000px;
  padding: 8px 13px;
  outline: none;
  cursor: pointer;
}
inc {
  background: white;
  color: black;
}
.submit {
  background: black;
  color: white;
  margin-left: 20px;
  padding: 12px 14px;
  width: 240px;
  transition: 0.25s all ease-in;
}
.submit:hover {
  opacity: 0.8;
  transition: 0.25s all ease-out;
}

.quant-text {
  display: inline-block;
  text-align: center;
  width: 140px;
  padding: 8px;
  padding: 8px;
}

.quantity {
  border: 2px solid black;
  width: 235px;
  padding-left: 3px;
  border-radius: 1000px;
  background: #fff;
  margin-left: 20px;
}

.item {
  display: flex;
  flex-direction: column;
  width: 280px;
  height: 400px;
  justify-content: space-around;
  background: #eee;
  padding: 20px 10px;
  margin: 30px;
}
</style>
