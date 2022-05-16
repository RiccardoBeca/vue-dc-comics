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
          <button><a href="#">LOAD MORE</a></button>
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



 .prova{
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100px;
    background-color: rgb(28, 28, 28);
    padding: 40px;
  } 
  .cards-container{
    display: flex;
    flex-wrap: wrap;
    position: relative;
    button{
    position: absolute;
    top: 95%;
    left: 50%;
    transform: translate(-50%);
    border-style: none;
    border: 2px solid $project-color;
    padding: 5px 40px;
    background-color: $project-color;
    a{
      font-size: 17px;
      color: white;
      text-decoration: none;
    }
  }
  }
  .jumbotron{
    height: 400px;
    background-image: url(../assets/img/jumbotron.jpg);
  }



</style>