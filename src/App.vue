<template>
  <div id="app">
    <h1>{{ title }}</h1>
    <ul>
      <li v-for="photo of photos">
        <img v-bind:src="photo.url" v-bind:alt="photo.titulo">
      </li>
    </ul>    
  </div>
</template>

<script>
export default {
  data () {
    return {
      title: 'Alurapic',
      photos: [
        {
          url: 'https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQJx-b8pkUH5XODzW0YoDoAPGUn5L8z7bgO7xaCDCbZNu74F6qK',
          title: 'Happy dog'
        },
        {
          url: 'https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQJx-b8pkUH5XODzW0YoDoAPGUn5L8z7bgO7xaCDCbZNu74F6qK',
          title: 'Happy dog'
        }
      ]
    }
  },
  created() {
    this.$http.get
  }
}
</script>

<style>
</style>
