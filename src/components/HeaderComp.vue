<template>
  <header>
    <div class="container w-70">
      <div class="logo">
       <img src="../assets/img/dc-logo.png" alt="DC Logo">
      </div>
      <nav>
        <ul>
        <li v-for="(item, index) in itemsList" :key="`nav-${index}`">
        <a :class="{'active':item.isActive}" :href="item.href">{{item.name}}</a></li>
      </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name:"HeaderComp",
  data(){
    return{
      itemsList:[
        {
          name: "CHARACTERS",
          href: "#",
          isActive: false,
        },
        {
          name: "COMICS",
          href: "#",
          isActive: true,
        },
         {
          name: "MOVIES",
          href: "#",
          isActive: false,
        },
         {
          name: "TV",
          href: "#",
          isActive: false,
        },
         {
          name: "GAMES",
          href: "#",
          isActive: false,
        },
         {
          name: "COLLECTIBLES",
          href: "#",
          isActive: false,
        },
         {
          name: "VIDEOS",
          href: "#",
          isActive: false,
        },
         {
          name: "FANS",
          href: "#",
          isActive: false,
        },
         {
          name: "NEWS",
          href: "#",
          isActive: false,
        },
         {
          name: "SHOP",
          href: "#",
          isActive: false,
        },
        
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/_vars.scss';
@import '../assets/style/_general.scss';
@import '../assets/style/_utils.scss';

  header {
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: white;
    padding: 20px;
    .logo{
      display: flex;
    }
    nav{
      display: flex;
      align-items: center;
      ul{
        display: flex;
        list-style: none;
      }
      li a{
        font-weight: bold;
        text-decoration: none;
        color: #53514c;
        margin: 15px;
        &:hover{
          color: $project-color;
          border-bottom: 3px solid $project-color;
          padding-bottom: 40px;
        }
        &.active{
          color: $project-color;
          border-bottom: 3px solid $project-color;
          padding-bottom: 40px;
        }
      }  
    }
  }
</style>