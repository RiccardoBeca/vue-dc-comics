<template> 

  <div>
    <HeaderComp />
    <MainComp />
    <FooterComp />
  </div>

</template>

<script>

import HeaderComp from "../src/components/HeaderComp.vue"
import MainComp from "../src/components/MainComp.vue"
import FooterComp from "../src/components/FooterComp.vue" 

export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    FooterComp
}
}
</script>

<style lang="scss">
@import './assets/style/vars';
@import './assets/style/general';
@import './assets/style/utils';

</style>
