<template>

    <div id="Information" >
      <div v-for="info in projects" :key="info.language">
        <div class="flex-container">
        <div class="Information">
          <div v-bind:class="info.language">
            <img v-bind:src="info.img" style="width: 200px; height: 200px" />
            <h1 class="pastel2">{{ info.language }} Professional</h1>
          </div>
        </div>
      </div>
  </div>
  </div>
</template>

<script>
export default {
  name: "Information",
  projects: [],
  data() {
    return {
      projects: [
        {
          img:
            "https://cdn3.iconfinder.com/data/icons/logos-and-brands-adobe/512/267_Python-512.png",
          language: "Python",
        },
        {
          img: "https://rustacean.net/assets/cuddlyferris.png",
          language: "Rust",
        },
           {
          img: "https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Vue.js_Logo_2.svg/1184px-Vue.js_Logo_2.svg.png",
          language: "Vue",
        },
           {
          img: "https://infinapps.com/wp-content/uploads/2018/10/mongodb-logo.png",
          language: "MongoDB",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.Python {
  color: black;
  background: #c3d2e5;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 200px;
}

.Rust {
  color: black;
  background: #ffb7b2;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 200px;
}
.Vue {
  color: black;
  background:   #E2F0CB;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 200px;
}

.MongoDB {
  color: black;
  background: #B5EAD7;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 200px;
}
.pastel1 {
  color: black;
  background: #c3d2e5;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 200px;
}
.pastel2 {
  color: black;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  border-radius: 2px;
  opacity: 20;
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
  display: flex;
  flex-direction: row;
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

.grid {
  display: grid;
  grid-template-columns: 1fr auto minmax(100px, 1fr) 1fr;
  grid-template-rows: 100px repeat(3, auto) 100px;
  grid-gap: 10px;
}
</style>