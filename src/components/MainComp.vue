<template>
  <main>
    <div class="jumbotron"></div>
     <div class="prova">
       <div class="w-70 cards-container">
          <CardComp
           v-for="(book, index) in booksList" :key="`book${index}`"
           :thumb="book.thumb"
           :series="book.series"
          />
        </div>
    </div>
    
  </main>
</template>

<script>
import CardComp from "./CardComp.vue";
import booksList from "../assets/data/booksLists";
export default {
    name: "MainComp",
    components: { CardComp },
    data() {
        return {
          booksList
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/_vars.scss';
@import '../assets/style/_general.scss';
@import '../assets/style/_utils.scss';

main{

 .prova{
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100px;
    background-color: rgb(28, 28, 28);
    padding: 40px;
  .cards-container{
    flex-wrap: wrap;
  }
  } 
  .jumbotron{
    height: 400px;
    background-image: url(../assets/img/jumbotron.jpg);
  }
}

</style>