
<template>
  <div class="About">
    <div class="flex-container">
      <div class="flex-container">
        <h1 class="pastel1" @click="render_about">about</h1>
      </div>
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

    <div v-if="which_stuff === 'about'"><Information /></div>
    <div v-if="which_stuff === 'links'">ToDo Links</div>
  </div>
</template>

<script>
import Information from "./Information.vue";

export default {
  name: "About",
  which_stuff: "none",
  data() {
    return {
      which_stuff: "none",
    };
  },
  methods: {
    render_about: function () {
      this.which_stuff = "about";
    },
    render_links: function () {
      this.which_stuff = "links";
    },
  },
  components: {
    Information,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.pastel1 {
  color: black;
  //background:#C7CEEA;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 140px;
}
.pastel2 {
  color: black;
  //background: #ffb7b2;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 140px;
}
.pastel3 {
  color: black;
  //background: #E2F0CB;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 140px;
}
.pastel4 {
  color: black;
  //background: #B5EAD7;
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