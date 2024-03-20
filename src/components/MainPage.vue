<template>
    <main-header></main-header>
    <main>
      <img class="cloudImg" src="../assets/bigCloud.png" alt="">
      <main-block-one></main-block-one>
    </main>
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
  main {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .cloudImg {
    top: 215px;
    left: 15%;
    position: absolute;
  }
  @media (max-width: 1150px) {
    .cloudImg {
    width: 189px;
    height: 126px;
    top: 215px;
    left: 20%;
    position: absolute;
    }
  }
  @media (max-width: 730px) {
    .cloudImg {
    width: 148px;
    height: 96px;
    top: 140px;
    left: 17%;
    position: absolute;
  }
  }
</style>