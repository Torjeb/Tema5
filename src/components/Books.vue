<template>
     <div v-for="(book, index) in books" :class="'content__book' + (index)">
      <div><img v-bind:src="'public/images/' + book.cover" /></div>
      <div>{{ book.writers }}</div>
      <div :class="'content__booktitle' + (index)">{{ book.title }}</div>
   </div>
  
</template>

<script>
export default {
   data () {
      return {

      }
   },
   
   computed: {
      articleOne() {
         return this.$store.getters.getArticleOne;
         
      },

      articleTwo() {
         return this.$store.getters.getArticleTwo;
      },

      articleThree() {
         return this.$store.getters.getArticleThree;
      },

      books() {
         return this.$store.getters.getBooks;
      }
   }
}
</script>

<style>


</style>