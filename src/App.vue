<template>
  <div id="app">
    <SongList/>
    <PlayList/>
  </div>
</template>

<script>
import PlayList from './components/PlayList.vue'
import SongList from './components/SongList.vue'


export default {
  name: 'App',
  components: {
    SongList,
    PlayList
  },
  
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
  display: grid;
  grid-template-columns: repeat(2, 1fr)
}
</style>
