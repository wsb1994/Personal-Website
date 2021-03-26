<template>
  <div class="Paragraph">
    <div class="flexbox">
      <p>
        &emsp; Hello, I'm William Berry. I am a graduating Senior at the
        University of Kentucky. In particular I am actually the Outstanding
        Graduating Senior for Computer Science, which if you ask me, is kind of
        rad. I do a lot of cool coding stuff like building this website, which
        was done with Vue.js.
      </p>

      <p>
        &emsp; Some of the more fun things I've gotten to work on were the
        rendering SDK and client on next generation devices for the Disney+
        streaming service. Every time you go to watch WandaVision, or catch up
        on what's happening to Baby Yoda on PS5, Xbox, your smart TV, or even
        your browser, you will in part have myself and my former coworker Elaine
        to thank for the smooth performance of the application.
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
        Cathacks VII! It's been a ton of fun. I can't believe I'm already
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
export default {
  name: "Paragraph",
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.Paragraph {
  color: black;
  font-size: 40px;
  text-align: center;
  margin-left: auto;
  margin-right: auto;
  width: 65%;

}
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

p{
  padding-bottom: 50px;
}


@media screen and (max-width: 1000px) {
.flexbox {
  align-items: center;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
}
.Paragraph {
  color: black;
  font-size: 30px;
  text-align: center;

}
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
}
</style>
