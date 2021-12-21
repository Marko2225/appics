<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    <router-view/>
  </div>
</template>

<style lang="scss"  >

$primary-color-dark: #12192C;
$primary-color: #1F273E;

* {
  box-sizing: border-box;
}

html, body {
  background-color: $primary-color;
  padding: 0px !important;
  margin: 0px !important;
  line-height: 24px;
}

#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: $primary-color;

}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

 @font-face {
      font-family: "Gotham";
      font-style: normal;
      font-weight: 900;
      src: url("../src/assets/fonts/gotham/Gotham-Black.eot?") format("eot"), url("../src/assets/fonts/gotham/Gotham-Black.woff2") format("woff2"), url("../src/assets/fonts/gotham/Gotham-Black.woff") format("woff"), url("../src/assets/fonts/gotham/Gotham-Black.ttf") format("truetype"), url("../src/assets/fonts/gotham/Gotham-Black.svg#Gotham") format("svg");
    }

    @font-face {
      font-family: "Gotham";
      font-style: normal;
      font-weight: bold;
      src: url("../src/assets/fonts/gotham/Gotham-Bold.eot?") format("eot"), url("../src/assets/fonts/gotham/Gotham-Bold.woff2") format("woff2"), url("../src/assets/fonts/gotham/Gotham-Bold.woff") format("woff"), url("../src/assets/fonts/gotham/Gotham-Bold.ttf") format("truetype"), url("../src/assets/fonts/gotham/Gotham-Bold.svg#Gotham") format("svg");
    }

    @font-face {
      font-family: "Gotham";
      font-style: normal;
      font-weight: 500;
      src: url("../src/assets/fonts/gotham/Gotham-Medium.eot?") format("eot"), url("../src/assets/fonts/gotham/Gotham-Medium.woff2") format("woff2"), url("../src/assets/fonts/gotham/Gotham-Medium.woff") format("woff"), url("../src/assets/fonts/gotham/Gotham-Medium.ttf") format("truetype"), url("../src/assets/fonts/gotham/Gotham-Medium.svg#Gotham") format("svg");
    }

    @font-face {
      font-family: "Gotham";
      font-style: normal;
      font-weight: normal;
      src: url("../src/assets/fonts/gotham/Gotham-Book.eot?") format("eot"), url("../src/assets/fonts/gotham/Gotham-Book.woff2") format("woff2"), url("../src/assets/fonts/gotham/Gotham-Book.woff") format("woff"), url("../src/assets/fonts/gotham/Gotham-Book.ttf") format("truetype"), url("../src/assets/fonts/gotham/Gotham-Book.svg#Gotham") format("svg");
    }

    @font-face {
      font-family: "Gotham";
      font-style: normal;
      font-weight: 300;
      src: url("../src/assets/fonts/gotham/Gotham-Light.eot?") format("eot"), url("../src/assets/fonts/gotham/Gotham-Light.woff2") format("woff2"), url("../src/assets/fonts/gotham/Gotham-Light.woff") format("woff"), url("../src/assets/fonts/gotham/Gotham-Light.ttf") format("truetype"), url("../src/assets/fonts/gotham/Gotham-Light.svg#Gotham") format("svg");
    }

    @font-face {
      font-family: "Gotham";
      font-style: normal;
      font-weight: 100;
      src: url("../src/assets/fonts/gotham/Gotham-Thin.eot?") format("eot"), url("../src/assets/fonts/gotham/Gotham-Thin.woff2") format("woff2"), url("../src/assets/fonts/gotham/Gotham-Thin.woff") format("woff"), url("../src/assets/fonts/gotham/Gotham-Thin.ttf") format("truetype"), url("../src/assets/fonts/gotham/Gotham-Thin.svg#Gotham") format("svg");
    }

</style>
