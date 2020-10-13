<template>
  <div id="app">
    <img src="./assets/logo.png">
    <div class="hello">
      <h1>{{ msg }}</h1>
      <ul>
        <li v-for="item in 7">{{item}}</li>
      </ul>
    </div>
    <router-view></router-view>
    <router-link to="/two" >第二个</router-link>
    <router-link to="/three" >第三个</router-link>
  </div>
</template>

<script>
export default {
  name: 'App',
  data(){
    return{
      msg:"大漠孤烟直"
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
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
a {
  color: #42b983;
}
</style>
