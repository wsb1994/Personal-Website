<template>
  <div id="Information">
    <div class="flex-container">
      <div v-for="info in projects" :key="info.language">
        <div class="Information">
          <div v-bind:class="info.color">
            <img v-bind:src="info.img" style="width: 75; height: 95px" />
            <h1 class="pastel2">{{ info.language }}</h1>
            <h1 class="white">{{ info.exp }}</h1>
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
          color: "black",
          exp: "@CPlan-IT",
        },
        {
          img: "https://rustacean.net/assets/cuddlyferris.png",
          language: "Rust",
          color: "black",
          exp: "@Disney+",
        },
        {
          img:
            "https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Vue.js_Logo_2.svg/1184px-Vue.js_Logo_2.svg.png",
          language: "Vue",
          color: "black",
          exp: "@Cplan-IT",
        },
        {
          img:
            "https://infinapps.com/wp-content/uploads/2018/10/mongodb-logo.png",
          language: "MongoDB",
          color: "black",
          exp: "@Cplan-IT",
        },
        {
          img:
            "https://blog.iron.io/wp-content/uploads/2016/01/docker-logo.png",
          language: "Docker",
          color: "black",
          exp: "@ViacomCBS",
        },
        {
          img:
            "https://www.probytes.net/wp-content/uploads/2018/10/flask-logo-png-transparent.png",
          language: "Flask",
          color: "black",
          exp: "@Cplan-IT",
        },
        {
          img: "https://www.a2go.org/images/logo.png",
          language: "Go",
          color: "black",
          exp: "@ViacomCBS",
        },
        {
          img: "https://symfony.com/logos/symfony_black_03.png",
          language: "Symfony",
          color: "black",
          exp: "@ViacomCBS",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.blue {
  color: black;
  background: #c3d2e5;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 100;
}

.black {
  color: Black;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 100;
}


.pink {
  color: black;
  background: #ffb7b2;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 100;
}
.Vue {
  color: black;
  background: #c3d2e5;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 100;
}

.green {
  color: black;
  background: #b5ead7;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 100;
}

.White {
  color: black;
  background: white;
  font-family: "Georgia", "Times New Roman", Times, serif, serif;
  padding: 16px;
  border-style: solid;
  border-radius: 30px;
  width: 100;
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
  padding-top: 100px;
  padding-bottom: 400px;
  align-items: center;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-around;
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