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
            "https://cdn3.iconfinder.com/data/icons/logos-and-brands-adobe/512/267_Python-512.png",
          language: "Python",
          color: "blue",
          exp: "@CPlan-IT",
        },
        {
          img: "https://rustacean.net/assets/cuddlyferris.png",
          language: "Rust",
          color: "pink",
          exp: "@Disney+",
        },
        {
          img:
            "https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Vue.js_Logo_2.svg/1184px-Vue.js_Logo_2.svg.png",
          language: "Vue",
          color: "green",
          exp: "@Cplan-IT",
        },
        {
          img:
            "https://infinapps.com/wp-content/uploads/2018/10/mongodb-logo.png",
          language: "MongoDB",
          color: "green",
          exp: "@Cplan-IT",
        },
        {
          img:
            "https://blog.iron.io/wp-content/uploads/2016/01/docker-logo.png",
          language: "Docker",
          color: "blue",
          exp: "@ViacomCBS",
        },
        {
          img:
            "https://www.probytes.net/wp-content/uploads/2018/10/flask-logo-png-transparent.png",
          language: "Flask",
          color: "blue",
          exp: "@Cplan-IT",
        },
        {
          img:
            "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fcamo.githubusercontent.com%2F98ed65187a84ecf897273d9fa18118ce45845057%2F68747470733a2f2f7261772e6769746875622e636f6d2f676f6c616e672d73616d706c65732f676f706865722d766563746f722f6d61737465722f676f706865722e706e67&f=1&nofb=1",
          language: "Go",
          color: "blue",
          exp: "@ViacomCBS",
        },
        {
          img: "https://symfony.com/logos/symfony_black_03.png",
          language: "Symfony",
          color: "pink",
          exp: "@ViacomCBS",
        },
        {
          img:
            "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fpytorch.org%2Fassets%2Fimages%2Fpytorch-logo.png&f=1&nofb=1",
          language: "Pytorch",
          color: "pink",
          exp: "@Research",
        },
        {
          img:
            "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2Fthumb%2F2%2F2d%2FTensorflow_logo.svg%2F449px-Tensorflow_logo.svg.png&f=1&nofb=1",
          language: "Tensorflow",
          color: "pink",
          exp: "@Research",
        },
        {
          img:
            "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fmaxcdn.icons8.com%2FShare%2Ficon%2FLogos%2Fcss31600.png&f=1&nofb=1",
          language: "CSS",
          color: "blue",
          exp: "@Projects",
        },
        {
          img:
            "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2Fthumb%2F0%2F00%2FHTML5_logo_black.svg%2F1200px-HTML5_logo_black.svg.png&f=1&nofb=1",
          language: "HTML5",
          color: "blue",
          exp: "@Projects",
        },
        {
          img:
            "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Flogos-download.com%2Fwp-content%2Fuploads%2F2016%2F09%2FGitHub_logo.png&f=1&nofb=1",
          language: "Git",
          color: "blue",
          exp: "@Everywhere!",
        },
        {
          img:
            "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2Fthumb%2F0%2F0d%2FC_Sharp_wordmark.svg%2F464px-C_Sharp_wordmark.svg.png&f=1&nofb=1",
          language: "C#",
          color: "blue",
          exp: "@Rawlings",
        },
        {
          img:
            "https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fwiki.sei.cmu.edu%2Fconfluence%2Fdownload%2Fthumbnails%2F88042725%2FC%2520Logo.png%3Fversion%3D1%26modificationDate%3D1527685155000%26api%3Dv2&f=1&nofb=1",
          language: "C",
          color: "blue",
          exp: "@Disney+",
        },
        {
          img:
            "https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fwww.freepngimg.com%2Fdownload%2Fc%2B%2B%2F2-2-c%2B%2B-png-clipart.png&f=1&nofb=1",
          language: "C++",
          color: "blue",
          exp: "@Disney+",
        },
        {
          img:
            "https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fsqlbackupandftp.com%2Fblog%2Fwp-content%2Fuploads%2F2015%2F01%2Fmysql-logo_2800x2800_pixels1-1024x1024.png&f=1&nofb=1",
          language: "mySQL",
          color: "blue",
          exp: "@Rawlings",
        },
        {
          img:
            "https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fwww.sqlalchemy.org%2Fimg%2Ftidelift.png&f=1&nofb=1",
          language: "SqlAlchemy",
          color: "blue",
          exp: "@Cplan-IT",
        },
        {
          img:
            "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdwglogo.com%2Fwp-content%2Fuploads%2F2017%2F12%2F1100px_Redis_Logo_01.png&f=1&nofb=1",
          language: "redis",
          color: "pink",
          exp: "@Projects",
        },
        {
          img:
            "https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fcdn.onlinewebfonts.com%2Fsvg%2Fimg_27628.png&f=1&nofb=1",
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
  align-items: left;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: flex-start;
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
