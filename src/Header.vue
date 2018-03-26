<template>
  <div id="header">
      <div class="logo">HJs</div>
      <h1>HackerJobs</h1>
      <div class="links">
          <a href ="/new">New</a>
          <a href = "/top">Top</a>
          <button id="filters">Filters</button>
          <a href="/submit">Submit</a>
          <button v-on:click="clickLogin" id="login">Login</button>
          <div v-if="loggingIn" class="login-fields">
              <a href="/register">New user?</a>
              <input id="username" placeholder="username"></input>
              <input id="password" placeholder="password"></input>
              <button id="login-button">Submit</button>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'header',
    data () {
        return {
            msg: 'Welcome to Your Vue.js App',
            loggingIn: false
        }
    },
    methods: {
        clickLogin: function() {
            console.log("Logging in?");
            this.loggingIn = true;
        }
    }
}
</script>

<style>
#header {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin-top: 60px;
  margin-left: 0;
  margin-right: 0;
  width: 100%;
  margin: 0;
  height: 10%;
  background-color: #fe6501;
  position: relative;
}

.logo {
    border: solid 1px white;
    display: inline-block;
    height: 30px;
    width: 30px;
    color: white;
}
#login {
    position: absolute;
    right: 0;
    top: 0;
    background: none;
    border: none;
    cursor: pointer;
}
.login-fields {
    border: 1px solid white;
    position: absolute;
    right: 0;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}
:focus {
    outline-width: 0;
}

a {
  color: #42b983;
}
</style>
