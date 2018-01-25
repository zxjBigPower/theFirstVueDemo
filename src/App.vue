<template>
  <div id="app">
    <img src="./assets/logo.png">
    {{msg}}
   <!-- <router-view/>-->
   <button @click="getJson">fdgedrge</button>
  </div>
</template>

<script>
export default {
	data (){
		return {
			msg :'\nasfdqfbnfgbnfgbnfnfdbfzbsfghsrfdhsweafd'
		}
	},
	methods:{
		getJson(){
			//console.log(222)
			this.$http.get("/data.json").then((res)=>{console.log(res),(err)=> {console.log(err)}})
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
</style>
