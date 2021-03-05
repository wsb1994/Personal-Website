<template>
  <div class="About">
    <div class="flex-container">
      <h1 class="pastel1" @click="render_about">About</h1>
      <h1 class="spacer"></h1>

      <h1 class="pastel1" @click="render_technology">Technologies</h1>
      <h1 class="spacer"></h1>

      <a href="https://github.com/wsb1994">
        <h1 class="pastel2">GitHub</h1>
      </a>
      <h1 class="spacer"></h1>

      <a href="https://www.linkedin.com/in/will-berry-8a65ab143/">
        <h1 class="pastel3">LinkedIn</h1>
      </a>
      <h1 class="spacer"></h1>

      <a
        href="https://docs.google.com/document/d/1gQG_9dNoqCEmzCrnREhRplIQEw8pRiRKeVOycAXQ-Ig/edit?usp=sharing"
      >
        <h1 class="pastel4">Resume</h1>
      </a>
      <h1 class="spacer"></h1>
    </div>

    <div v-if="which_stuff === 'technology'">
      <Technology />
    </div>

    <div v-if="which_stuff === 'about'">
      <p>
        &emsp; Hello, I'm William Berry. I am a graduating Senior at the
        University of Kentucky. In particular I am actually the Outstanding
        Graduating Senior for Computer Science, which if you ask me, is kind of
        rad. I do a lot of cool coding stuff like building this website, which
        was done with vue.js.
      </p>

      <p>
        &emsp; Some of the more fun things I've gotten to work on were the
        rendering SDK and client on next generation devices for the Disney+
        streaming service. Every time you go to watch WandaVision, or catch up
        on what's happening to Baby Yoda on PS5, Xbox, your telivision, or even
        your browser, you will in part have me to thank for the smooth
        performance of the application.
      </p>
      <p>
        &emsp; I also set up a good portion of the infrastructure that allows
        for seamless password resets in a server-less configuration for
        ViacomCBS across 53+ websites! I was able to consolidate all
        authorization and authentication requests into one api/transformer
        service to help scale with less resources. Nifty what the modern cloud
        can do!
      </p>
      <p>
        &emsp; I am also very active at UK. Being the former Vice President of
        Social Media for the Squirrel Watching Club (an outdoor activity club
        killed by covid I'm afraid), and the current 2021 Vice President of the
        Association for Computing Machinery. I also help out as one of the
        Hackathon Planning chairs, planning CatHacks: Winter Edition, and
        Cathacks VII! It's been a ton of fun. I can't beleive I'm already
        graduating, but it's been an absolutely wild ride. I'm still currently
        available to hire, and I specialize in cloud based back-end services for
        your business or organization.
      </p>

      <p>
        &emsp; To see what other cool stuff I've built, check out my
        technologies tab, or check out my github.
      </p>
    </div>
  </div>
</template>

<script>
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
    render_about: function() {
      this.which_stuff = "about";
    },
    render_technology: function() {
      this.which_stuff = "technology";
    },
  },

  components: {
    Technology,
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
  text-align: left;
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
  background: #ffb7b2;
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
  background: #e2f0cb;
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
  background: #b5ead7;
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
img{
  width: auto ;
  max-width: 50% ;
  height: auto ;
}
</style>
