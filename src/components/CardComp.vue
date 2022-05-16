<template>
  <div>
    <div class="img-container">
     <img :src="thumb" :alt="series">
    </div>
    <p>{{series}}</p>
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
  width: calc(100% / 6);
  padding-bottom: 50px;
}

p{
  font-size: .75rem;
  padding-top: 15px;
  color: white;
  text-transform: uppercase;
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