<template>
    <main-header></main-header>
    <main>
      <img class="cloudImg" src="../assets/cloud.png">
      <img class="cubeImg" src="../assets/blueCube.png">
      <img class="coneImg" src="../assets/pinkCone.png">
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
  main {
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .cloudImg {
    position: absolute;
    top: 115px;
    left: 15%;
    position: absolute;
  }
  .cubeImg {
    position: absolute;
    right: 0;
    top: 270px;
  }
  .coneImg {
    position: absolute;
    left: 2%;
    top: 1000px;
  }
  @media (max-width: 1150px) {
    .cloudImg {
    width: 189px;
    height: 126px;
    top: 115px;
    left: 20%;
    position: absolute;
  }
    .cubeImg {
    width: 119px;
    height: 134px;
    right: 1%;
    top: 210px;
  }
    .coneImg {
    width: 141px;
    height: 151px;
    top: 680px;
  }
  }
  @media (max-width: 730px) {
    .cloudImg {
      width: 148px;
      height: 96px;
      top: 40px;
      left: 17%;
      position: absolute;
    } 
    .cubeImg {
      top: 120px;
    }
    .coneImg {
      top: 500px;
    }
  }
  @media (max-width: 450px) {
    .cubeImg {
      width: 72px;
      height: 78px;
      right: 1%;
      top: 140px;
    }
    .coneImg {
      left: 0;
      top: 380px;
      width: 88px;
      height: 86px;
    } 
  }
</style>