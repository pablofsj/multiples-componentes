<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/chems.jpg">
    <HelloWorld msg="Lista de cosas random de Pablo"/>
    <ListaEnlaces titulo="Miembros de la familia Simpson" v-bind:enlaces="enlaces_simpson" />
    <ListaEnlaces titulo="Cosas que me gustaria comer ahora" v-bind:enlaces="enlaces_comidas" />
    <br> <br> <br>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import ListaEnlaces from './components/ListaEnlaces.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    ListaEnlaces
  },
  data: () => {
    return {
      // acá están mis datos
      enlaces_simpson: [
        {texto: 'Homero', url: 'https://es.wikipedia.org/wiki/Homer_Simpson'},
        {texto: 'Marge', url: 'https://es.wikipedia.org/wiki/Marge_Simpson'},
        {texto: 'Bart', url: 'https://es.wikipedia.org/wiki/Bart_Simpson'},
        {texto: 'Lisa', url: 'https://es.wikipedia.org/wiki/Lisa_Simpson'},
        {texto: 'Maggie', url: 'https://es.wikipedia.org/wiki/Maggie_Simpson'}

      ],
      enlaces_comidas: [
        {texto: 'Papas Fritas', url: 'https://es.wikipedia.org/wiki/Papas_fritas'},
        {texto: 'Tocomples', url: 'https://es.wikipedia.org/wiki/Completo_(gastronomía)'},
        {texto: 'Churrasco', url: 'https://es.wikipedia.org/wiki/Churrasco'},
        {texto: 'Empanadas', url: 'https://es.wikipedia.org/wiki/Empanada'},
        {texto: 'Sushi', url: 'https://es.wikipedia.org/wiki/Sushi'},
      
    ],
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


