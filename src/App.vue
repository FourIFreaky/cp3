<template>
  <div id="app">
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/car">The Cars</router-link> |
      <router-link to="/about">About</router-link>
    </nav>
    <router-view/>
    <div id="footer">
      <a href="https://github.com/FourIFreaky/cp3">Github Repository</a>
    </div>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: FireBrick;
}

#footer {
  text-align: left;
  position: absolute;
  bottom: 0;
  width: 100%;
}
</style>
