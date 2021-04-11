<template>
  <div id="Technology">
    <div class="flex-container">
      <div v-for="info in projects" :key="info.language">
        <div class="Information">
          <div v-bind:class="info.color">
            <img v-bind:src="info.img" style="width: 75; height: 95px" />
            <h1 class="header">{{ info.language }}</h1>
            <h1>{{ info.exp }}</h1>
            <h1 class="spacer"></h1>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Technology",
  projects: [],
  data() {
    return {
      projects: [
        {
          img:
            require("../public/assets/python.jpg"),
          language: "Python",
          color: "blue",
          exp: "@CPlan-IT",
        },
        {
          img:  require("../public/assets/rust.png"),
          language: "Rust",
          color: "pink",
          exp: "@Disney+",
        },
        {
          img:
            require("../public/assets/vue.png"),
          language: "Vue",
          color: "green",
          exp: "@Cplan-IT",
        },
        {
          img:
            require("../public/assets/mongo.png"),
          language: "MongoDB",
          color: "green",
          exp: "@Cplan-IT",
        },
        {
          img:
            require("../public/assets/docker.png"),
          language: "Docker",
          color: "blue",
          exp: "@ViacomCBS",
        },
        {
          img:
            require("../public/assets/flask.png"),
          language: "Flask",
          color: "blue",
          exp: "@Cplan-IT",
        },
        {
          img:
            require("../public/assets/go.png"),
          language: "Go",
          color: "blue",
          exp: "@ViacomCBS",
        },
        {
          img: require("../public/assets/symfony.png"),
          language: "Symfony",
          color: "pink",
          exp: "@ViacomCBS",
        },
        {
          img:
            require("../public/assets/css.png"),
          language: "CSS",
          color: "blue",
          exp: "@Projects",
        },
        {
          img:
           require("../public/assets/html.png"),
           language: "html",
          color: "blue",
          exp: "@Projects",
        },
        {
          img:
            require("../public/assets/git.png"),
          language: "git",
          color: "blue",
          exp: "@Everywhere!",
        },
        {
          img:
           require("../public/assets/csharp.png"),
          language: "C#",
          color: "blue",
          exp: "@Rawlings",
        },
        {
          img:
           require("../public/assets/c.png"),
           language: "C",
          color: "blue",
          exp: "@Disney+",
        },
        {
          img:
            require("../public/assets/cplusplus.png"),
          language: "C++",
          color: "blue",
          exp: "@Disney+",
        },
        {
          img: require("../public/assets/sql.png"),
          language: "mySQL",
          color: "blue",
          exp: "@Rawlings",
        },
        {
          img:
          require("../public/assets/sqlalchemy.png"),
          language: "SqlAlchemy",
          color: "blue",
          exp: "@Cplan-IT",
        },
        {
          img:
            require("../public/assets/redis.png"),
          language: "redis",
          color: "pink",
          exp: "@Projects",
        },
        {
          img:
            require("../public/assets/math.png"),
          language: "Math",
          color: "blue",
          exp: "@Everywhere!",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.black {
  color: Black;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 16px;
  font-size: 14px;
  border-style: solid;
  border-radius: 30px;
  width: 100;
  margin-left: 10px;
  margin-right: 10px;
  margin-top: 30px;
}

.black:hover {
  color: Black;
  background: #ffb7b2;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 16px;
  font-size: 14px;
  border-style: solid;
  border-radius: 30px;
  width: 100;
  margin-left: 10px;
  margin-right: 10px;
  margin-top: 30px;
}

.blue {
  color: Black;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 16px;
  font-size: 14px;
  border-style: solid;
  border-radius: 30px;
  width: 100;
  margin-left: 10px;
  margin-right: 10px;
  margin-top: 30px;
}

.blue:hover {
  color: Black;
  background: #c7ceea;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 16px;
  font-size: 14px;
  border-style: solid;
  border-radius: 30px;
  width: 100;
  margin-left: 10px;
  margin-right: 10px;
  margin-top: 30px;
}

.pink {
  color: Black;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 16px;
  font-size: 14px;
  border-style: solid;
  border-radius: 30px;
  width: 100;
  margin-left: 10px;
  margin-right: 10px;
  margin-top: 30px;
}

.pink:hover {
  color: Black;
  background: #ff9aa2;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 16px;
  font-size: 14px;
  border-style: solid;
  border-radius: 30px;
  width: 100;
  margin-left: 10px;
  margin-right: 10px;
  margin-top: 30px;
}

.green {
  color: Black;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 16px;
  font-size: 14px;
  border-style: solid;
  border-radius: 30px;
  width: 100;
  margin-left: 10px;
  margin-right: 10px;
  margin-top: 30px;
}

.green:hover {
  color: Black;
  background: #b5ead7;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 16px;
  font-size: 14px;
  border-style: solid;
  border-radius: 30px;
  width: 100;
  margin-left: 10px;
  margin-right: 10px;
  margin-top: 30px;
}

.header {
  color: black;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  border-radius: 2px;
  opacity: 20;
  width: 195px;
}

.flex-container {
  padding-top: 100px;
  padding-bottom: 400px;
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
