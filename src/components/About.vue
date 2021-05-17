<template>
  <div class="About">
    <div class="flex-container">
      <h1 class="pastel1" @click="render_about">About</h1>
      <h1 class="spacer"></h1>

      <h1 class="pastel2" @click="render_technology">Technologies</h1>
      <h1 class="spacer"></h1>

      <a href="https://github.com/wsb1994">
        <h1 class="pastel3">GitHub</h1>
      </a>
      <h1 class="spacer"></h1>

      <a href="https://www.linkedin.com/in/will-berry-8a65ab143/">
        <h1 class="pastel4">LinkedIn</h1>
      </a>
      <h1 class="spacer"></h1>

      <a
        href="https://drive.google.com/file/d/10R1LDRGtCkib8xVlUUIabgAHcU15fHJA/view?usp=sharing"
      >
        <h1 class="pastel5">Resume</h1>
      </a>
      <h1 class="spacer"></h1>
    </div>

    <div v-if="which_stuff === 'technology'">
      <Technology />
    </div>

    <div v-if="which_stuff === 'about'">
     <Paragraph />
    </div>
  </div>
</template>

<script>
import Paragraph from './Paragraph.vue';
import Technology from "./Technology.vue";

export default {
  name: "About",
  which_stuff: "default",

  data() {
    return {
      which_stuff: "default",
    };
  },

  methods: {
    render_about: function () {
      this.which_stuff = "about";
    },
    render_technology: function () {
      this.which_stuff = "technology";
    },
  },

  components: {
    Technology,
    Paragraph
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  color: black;
  padding-top: 35px;
}
p {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  color: black;
  font-size: 25px;
  text-align: center;
  max-width: 100%;
}
.pastel1 {
  color: black;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 200px;
}
.pastel1:hover {
  color: black;
  background: #c7ceea;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 200px;
}
.pastel2 {
  color: black;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 200px;
}
.pastel2:hover {
  color: black;
  background: #B5EAD7;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 200px;
}
.pastel3 {
  color: black;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 200px;
}
.pastel3:hover {
  color: black;
  background: #E2F0CB;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 200px;
}
.pastel4 {
  color: black;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 200px;
}

.pastel4:hover {
  color: black;
  background: #FFDAC1;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 200px;
}

.pastel5 {
  color: black;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 200px;
}

.pastel5:hover {
  color: black;
  background: #FFB7B2;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 200px;
}
.spacer {
  padding: 8px;
}

.flex-container {
  align-items: center;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
}

.flex-column {
  align-items: center;
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  justify-content: center;
}

a:link {
  text-decoration: none;
}

a:visited {
  text-decoration: none;
}

a:active {
  text-decoration: underline;
}
</style>
