<template>
  <w-app id="app">
    <header>Header</header>
    <w-flex grow>
      <aside>
        <div id="nav">
          <router-link to="/">Home</router-link> |
          <router-link to="/about">About</router-link>
        </div>
      </aside>
      <main class="grow">
        <router-view/>
      </main>
    </w-flex>
    <footer>Footer</footer>
  </w-app>
</template>

<style lang="scss">
@import '~wave-ui/dist/wave-ui.css';

body {
  background-color: rgb(255, 255, 198);
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
