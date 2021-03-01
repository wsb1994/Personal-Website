<template>
 <div class="flex-container">
  <div class="Information">
      <div class='pastel1'>
      <img src="https://cutewallpaper.org/21/big-chungus-picture/Big-Chungus-that-you-can-print-and-color-it.-BigChungus.jpg"  style="width:200px;height:200px;">
      <h1 class='pastel2'> Wungus </h1>
      </div>
  </div>
  </div>
</template>

<script>
export default {
  name: "Information",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.pastel1 {
  color: black;
  background: #ff9aa2;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  padding: 16px;
  border-style: solid;
  width: 200px;
}
.pastel2 {
  color: black;
  background: #ffb7b2;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  border-style: solid;
  width: 195px;

}
.pastel3 {
  color: black;
  background: #ffdac1;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  padding: 16px;
  border-style: solid;

  width: 140px;
}
.pastel4 {
  color: black;
  background: #e2f0cb;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 140px;
}
.spacer {
  color: black;
  padding: 32px;
}

.flex-container {
  align-items:center;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
}

a:link {
  text-decoration: none;
}

a:visited {
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}

a:active {
  text-decoration: underline;
}
</style>