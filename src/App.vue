<template>
  <div id="app">
    <!-- <header class="site-header">
      <div class="wrapper site-header__wrapper">
        <a href="#" class="brand"><img src="logo.svg" alt="brand" /></a>
        <nav class="nav"></nav>
      </div>
    </header> -->
    <div id="nav" class="header-area">
      <ul class="header-menu">
        <li><router-link to="/"><img src="favicon.ico" alt="brand" /></router-link></li>

        <!-- TODO: 一旦全routerを表示しておく。後で削除。 -->
        <li><router-link to="/login">Login</router-link></li>
        <li><router-link to="/logout">Logout</router-link></li>
        <li><router-link to="/signup">Signup</router-link></li>
      </ul>
    </div>
    <router-view />
  </div>
</template>

<style>
body {
	margin: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;

}

.header-area {
  background-color: #deffef;
}

.header-menu {
  display: flex;
  flex-wrap: wrap;
  list-style-type: none;
  margin: 0;
}

li {
  display: block;
  padding: 1.5rem 1rem;
}

</style>
