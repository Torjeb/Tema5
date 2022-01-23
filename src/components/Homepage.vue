<template>
<div class="content__mainart">
  <h2>{{  articleOne.title }}</h2>
  <div>{{ articleOne.lead }}</div>
  <img v-bind:src="'public/images/' + articleOne.preview.image" /> 
</div>

<div class="content__secart">
   <h2>{{  articleTwo.title }}</h2>
  <div>{{ articleTwo.lead }}</div>
  <img v-bind:src="'public/images/' + articleTwo.preview.image" /> 
</div>  

<div class="content__thirdart">
   <h2>{{  articleThree.title }}</h2>
  <div>{{ articleThree.lead }}</div>
  <img v-bind:src="'public/images/' + articleThree.preview.image" />
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
   }
}

</script>

<style>

</style>