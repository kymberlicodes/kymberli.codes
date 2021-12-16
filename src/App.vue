<template>
  <div id="app">
    <div id="nav">
      <img src="../src/assets/logo.png" class="logo">
      <router-link to="/">Home</router-link>
      <router-link to="/about">About</router-link>
      <router-link to="/blog">Blog</router-link>
      <router-link to="/contact">Contact</router-link>
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">
#app {
  font-family: 'Montserrat', sans-serif;
  font-weight: 200;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

a {
  font-family: 'Montserrat', sans-serif;
  font-weight: 200;
}

h1 {
  font-weight: 400;
}

h2 {
  font-weight: 400;
}

#nav {
  padding: 30px;
  display: flex;
  justify-content: space-between;
  align-items: center;

  a {
    font-weight: 400;
    color: #2c3e50;
    text-decoration: none;

    &.router-link-exact-active {
      color: #42b983;
    }

    &:hover {
      text-decoration: underline;
    }
  }

  .logo {
    max-width: 325px;
  }
}
</style>
