<template>
  <div class="block">
    <p class="blockText">Начни заниматься прямо<br><snap class="blockTextStrong">сейчас</snap></p>
    <button class="blockBtn">Начать</button>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
  .block {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin-top: 411px;
    width: 100%;
    height:735px;
    background-size: cover;
    background-image: url("../assets/bigMainBack.png");
  }
  .blockText {
    color: #FFFFFF;
    font-weight: 500;
    text-align: center;
    font-size: 96px;  
  }
  .blockTextStrong {
    color: #05F0FF;
  }
  .blockBtn {
    margin-top: 50px;
    font-weight: 500;
    font-size: 48px;
    color: #FFFFFF;
    background-color: #D89CE1;
    border: 0px;
    border-radius: 100px;
    width: 350px;
    height: 108px;
  }
  .blockBtn:hover {
    cursor: pointer;
  }
  @media (max-width: 1150px) {
    .block {
    margin-top: 270px;
    height: 500px;
    background-image: url("../assets/MidMainBack.png");
  }
    .blockText {
      font-size: 56px;
  }
    .blockBtn {
      margin-top: 20px;
      font-size: 24px;
      width: 170px;
      height: 55px;
    }

  }
  @media (max-width: 730px) {
    .block {
    margin-top: 170px;
    height: 410px;
    background-image: url("../assets/MinMainBack.png");
  }
    .blockText {
    font-size: 39px;
  }
  }
  @media (max-width: 450px) {
    .block {
      height: 250px;
    }
    .blockText {
      font-size: 32px;
    }
  }
</style>