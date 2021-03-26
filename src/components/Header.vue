<template>
  <div class="Header">
    <img
      alt="Person coding and drinking coffee"
      src="../public/assets/coffee.jpg"
    />
    <h1>Coding With Will</h1>
  </div>
</template>

<script>
export default {
  name: "Header",
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

h1 {
  color: black;
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
img{
  width: auto ;
  max-width: 50%;
  height: auto ;
}
</style>
