<template>
<div class="">

</div>
</template>

<script>


export default {
  name: 'app',
  data(){
    return {
     filmData: ""
    }
  },
  mounted(){
    fetch("https://ghibliapi.herokuapp.com/films")
    .then(dataFilm => dataFilm.json())
    .then(dataFilm => this.filmData = dataFilm.file)
  },
  components: {

  }
}
</script>







<!-- CSS -->
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
