<template>
<img alt="git logo" src="./assets/git.png">

   <home_git/>

</template>

<script>
import home_git from './components/home_git.vue'


export default {
  name: 'App',
   
   components :{
              home_git
   }
  
  }

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
