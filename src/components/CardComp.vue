<template>
  <div>
    <div class="img-container">
     <img :src="thumb" :alt="series">
    </div>
    <h3>{{series}}</h3>
  </div>
</template>

<script>
export default {
  name: "booksCard",
  props: {
    thumb: String,
    series: String
  }
}
</script>

<style lang="scss" scoped>

div{
  flex-basis: 16.6%;
 
}
.img-container{
  height:150px;
  width: 150px;
  overflow:hidden;
  img{
    width: 100%;
  }
}


</style>