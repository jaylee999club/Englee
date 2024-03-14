<template>
  <div class="gradient"></div>
  <div class="linkBlock">
    <img src="../assets/logo.png" alt="logo">
    <a href="@" class="linkItem">Главная</a>
    <a href="@" class="linkItem">Сообщество</a>
    <a href="@" class="linkItem">Карточки</a>
    <button class="btn">Войти</button>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
  .gradient {
    background: linear-gradient(to right, #05F0FF, #590BD9);
    width: 100%;
    height: 10px;
  }
  .linkBlock {
    display: flex;
    align-items: center;
  }
  .linkItem {
    font-weight: 400;
    font-size: 20px;
    color: #590BD9;
    text-decoration: none;
  }
  .btn {
    color: #FFFFFF;
    background-color: #590BD9;
    opacity: 0.33;
    border-radius: 100px;
    padding: 10px 40px;
    font-weight: 500;
    font-size: 26px;
    border: 0px;
  }
  .btn:hover {
    cursor: pointer;
  } 
</style>