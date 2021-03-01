<template>
  <div class="About">
    <div class="flex-container">
      <h1 class="pastel1" @click="render_about">about</h1>
      <h1 class="spacer"></h1>
      <a href="https://github.com/wsb1994">
        <h1 class="pastel2">github</h1>
      </a>
      <h1 class="spacer"></h1>
      <h1 class="pastel3" @click="render_links">links</h1>
      <h1 class="spacer"></h1>
      <h1 class="pastel4">resume</h1>
      <h1 class="spacer"></h1>
    </div>

    <div v-if="which_stuff === 'about'"> ToDo About </div>
    <div v-if="which_stuff === 'links'"> ToDo Links </div>
  </div>
</template>

<script>
export default {
  name: "About",
  which_stuff: 'none',
 data() {
    return {
      which_stuff: 'none'
    }
 }
 ,
 methods:{
     render_about: function(){
         this.which_stuff = 'about'
     }
     ,
     render_links: function(){
         this.which_stuff = 'links'
     }
 },
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
  border-radius: 30px;
  width: 140px;
}
.pastel2 {
  color: black;
  background: #ffb7b2;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 140px;
}
.pastel3 {
  color: black;
  background: #ffdac1;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
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
  align-items: center;
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