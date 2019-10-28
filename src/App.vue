<template>
<div id="app">
<h1>Studio Ghibli films</h1>

</div>
</template>





<script>

import filmList from "./components/filmList.vue"

export default {
  name: 'app',
  data(){
    return {
     filmData: "",
     films: []
    }
  },
  methods: {
    fetch("https://ghibliapi.herokuapp.com/films")
    .then(dataFilm => dataFilm.json())
    .then(dataFilm => this.filmData = dataFilm.file)

  },
  components: {
   "studio-ghibli-film-list": filmList
  }
}

// computed, mounted, differences in between them 
</script>







<!-- CSS -->
<style>
#app {
  background-color: #6EC3F4;
}
#list-info {
  display: flex;
}
</style>
