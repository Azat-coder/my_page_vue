<template>
  <div class="app">
    <div v-bind:class="{nav: isNav}">
      <router-link to="/">Обо мне</router-link> 
      <router-link to="/work">Опыт работы</router-link>
      <router-link to="/biography">Биография</router-link>
      <router-link to="/contacts">Контакты</router-link>
    </div>
    <router-view/>
  </div>
</template>

<script>
export default {
  data() { return {
    isNav: true
   }
     
 }
}
</script>


<style>
.visually-hidden {
	position: absolute;
	width: 1px;
	height: 1px;
	margin: -1px;
	border: 0;
	padding: 0;
	white-space: nowrap;
	clip-path: inset(100%);
	clip: rect(0 0 0 0);
	overflow: hidden;
}

.app {
  font-family: PT Sans Narrow, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale; 
  text-align: center;
  color: #2c3e50;
}

.nav {
  padding: 20px;
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  max-width: 600px;
  margin: 0 auto;
}

.nav a {
  font-weight: bold;
  color: #2c3e50;
  margin-right: 10px;
  text-decoration: none;
  text-transform: uppercase;
  font-size: 1.5em;
}

.nav a.router-link-exact-active {
  color: #739e0c;;
}
</style>
