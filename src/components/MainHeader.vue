<template>
  <div class="gradient"></div>
  <div class="linkBlock">
    <img src="../assets/logo.png" alt="logo" class="logoImg">
    <div class="linkLine">
      <a href="@" class="linkItem">Главная</a>
      <a href="@" class="linkItem">Сообщество</a>
      <a href="@" class="linkItem">Карточки</a>
      <button class="btn">Войти</button>
      <div class="burgerMenu">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
  .gradient {
    background: linear-gradient(to right, #05F0FF, #A781E4);
    width: 100%;
    height: 10px;
  }
  .linkBlock {
    margin-top: 10px;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  .logoImg {
    margin-left: 90px;
  }
  .linkLine {
    display: flex;
    align-items: center;
    margin-right: 90px;
    justify-content: space-around;
  }
  .linkItem {
    font-weight: 500;
    margin: 0px 40px;
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
    font-weight: 700;
    font-size: 26px;
    border: 0px;
  }
  .btn:hover {
    cursor: pointer;
  }
  .burgerMenu {
    display:none;
  }
  @media (max-width: 1150px) {
    .gradient {
      height: 8px;
    }
    .linkBlock {
      margin-top: 4px;
    }
    .logoImg {
      height: 104px;
      width: 85px;
      margin-left: 32px;
    }
    .linkLine {
      margin-right: 15px;
    }
    .linkItem {
      margin: 0px 29px;
    }
  }
  @media (max-width: 730px) {
    .gradient {
      height: 6px;
    }
    .linkBlock {
      align-items: flex-start;
      margin-top: 2px;
    }
    .logoImg {
      height: 80px;
      width: 60px;
      margin-left: 25px;
    }
    .linkLine {
      margin-right: 25px;
    }
    .linkItem {
      display: none;
    }
    .btn {
      display: none;
    }
    .burgerMenu {
      margin-top: 25px;
      display: flex;
      justify-content: space-between;
      flex-direction: column;
      width: 40px;
      height: 30px;
      position: relative;
    }
    .burgerMenu:hover {
      cursor: pointer;
    }
    .burgerMenu span {
      width: 100%;
      height: 6px;
      background-color: #590BD9;
    }
  }
</style>