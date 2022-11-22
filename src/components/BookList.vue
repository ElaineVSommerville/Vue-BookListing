<template>
  <div>
    <h1>{{ title }}</h1>
    <li> v-for="book in books": {{ book.title }} : {{ book.author }}</li>
  </div>
</template>

<script>
export default {
  data() {
    return {
      title: 'All Books',
      books: [
        {title: 'Self-Reliance', author: 'Ralph Waldo Emerson'},
        {title: 'American Gods', author: 'Neil Gaiman'},
        {title: 'Amusing Ourselves to Death', author: 'Neil Postman'},
      ]
    }
  },
  name: 'BookList'
}
</script>

<style>
h1, h2 {
  font-weight: normal;
}
li {
  display: block;
  margin: 0 10px;
}
</style>
