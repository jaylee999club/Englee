<template>
    <main-header></main-header>
    <img class="cloudImg" src="../assets/bigMainPage/bigCloud.png" alt="">
    <main-block-one></main-block-one>
</template>

<script>
import MainHeader from '@/components/MainHeader.vue';
import MainBlockOne from '@/components/MainBlockOne.vue';
export default {
  components: { MainHeader, MainBlockOne },

}
</script>

<style scoped>
  template {
    position: relative;
  }
  .cloudImg {
    display: none;
    top: 215px;
    left: 15%;
    position: absolute;
  }
  main-block-one {
    display: none;
  }
</style>