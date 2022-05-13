<template>
  <main>
    <div class="w-70">
     <h2>-->Content goes here>--</h2>
    </div>
  </main>
</template>

<script>
export default {
  name:"MainComp"

}
</script>

<style lang="scss" scoped>
@import '../assets/style/_vars.scss';
@import '../assets/style/_general.scss';
@import '../assets/style/_utils.scss';

main{
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100px;
  background-color: black;
  h2{
    display: flex;
    justify-content: flex-start;
    color: white;
  }
}

</style>