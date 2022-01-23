<template>
<div class="content">
	<!-- <div class="content__mainart">

	</div>
	<div class="content__secart">

	</div>
	<div class="content__thirdart">

	</div> -->

	<Homepage />
	<div class="content__books">
		<Books />
	</div>
</div>




<!-- <Header /> -->
<!--   <Homepage />
  <Books />
  <Footer />
    -->
  
</template>

<script>
import Header from '../components/Header.vue'
import Homepage from '../components/Homepage.vue'
import Footer from '../components/Footer.vue'
import Books from '../components/Books.vue'

export default {
	components: {
		Header,
		Homepage,
		Footer,
		Books
	}
}
</script>

<style>


* {
	box-sizing: border-box;
	margin: 0;
	padding: 0;
	
}

.content {
	display: grid;
	margin: 0 auto;
	text-align: center;
	grid-template-columns: repeat(6, 1fr);
	grid-gap: 12px;
	width: 100%;
}

.content__mainart {
	grid-column: 1 / 7;
}

.content__secart {
	grid-column: 1 / 4;
}

.content__thirdart {
	grid-column: 4 / 7;
}
content__book0
.content__book0 {
	grid-column: 1 / 2;
}

.content__book1 {
	grid-column: 2 / 3;
}

.content__book2 {
	grid-column: 3 / 4;
}

.content__book3 {
	grid-column: 4 / 5;
}

.content__book4 {
	grid-column: 5 / 6;
}

.content__book5 {
	grid-column: 6 / 7;
}

</style>