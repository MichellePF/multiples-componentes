<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <MiLista titulo="Lenguajes Aprendidos:" v-bind:enlaces="lenguajes_aprendidos"/>
    <MiLista titulo="Lenguajes por Aprender:" v-bind:enlaces="lenguajes_por_aprender"/>
  </div>
</template>

<script>
import MiLista from './components/MiLista.vue'

export default {
  name: 'App',
  components: {
    MiLista
  },
   data: function(){
        return{
            lenguajes_aprendidos: [
              {texto:'HTML', url:"https://developer.mozilla.org/es/docs/HTML/HTML5"}, 
              {texto:'CSS', url:"https://desarrolloweb.com/manuales/css3.html"},
              {texto:'Vue', url:"https://vuejs.org/"},
            ],
            lenguajes_por_aprender: [
              {texto:'Python', url:"https://www.python.org/"}, 
              {texto:'Dart', url:"https://dart.dev/"},
              {texto:'React', url:"https://es.reactjs.org/"},
            ]
        }
       
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
