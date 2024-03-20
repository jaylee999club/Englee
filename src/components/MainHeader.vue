<template>
  <div class="gradient"></div>
  <div class="linkBlock">
    <img src="../assets/logo.png" alt="logo" class="logoImg">
    <div class="linkLine">
      <a href="@" class="linkItem">Главная</a>
      <a href="@" class="linkItem">Сообщество</a>
      <a href="@" class="linkItem">Карточки</a>
      <button class="btn">Войти</button>
      <div class="burgerMenu" @click="open">
        <span></span>
        <span></span>
        <span></span>
      </div>
      <div class="menu">
        <div class="menuLink">Главная</div>
        <div class="menuLink">Сообщество</div>
        <div class="menuLink">Карточки</div>
        <div class="menuLink menuBtn">Войти</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    open() {
      let menu = document.querySelector('.menu');
      if (menu.classList.contains('.open')) {
        menu.classList.remove('.open');
        menu.style.display = "none";
      } else {
        menu.classList.add('.open');
        menu.style.display = "flex";
      }
    }
  }

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
  .menu {
    display: none;
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
      width: 70px;
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
      display: block;
      margin-top: 25px;
      width: 40px;
      height: 30px;
      position: relative;
      z-index: 3;
    }
    .burgerMenu:hover {
      cursor: pointer;
    }
    .burgerMenu span {
      position: absolute;
      width: 100%;
      height: 6px;
      background-color: #590BD9;
    }
    .burgerMenu span:nth-child(2) {
      top: 12px;
    }
    .burgerMenu span:nth-child(3) {
      bottom: 0px;
    }
    .menu {
      display: none;
      flex-direction: column;
      position: absolute;
      top: 6px;
      right: 0px;
      width: 300px;
      height: auto;
      padding-top: 70px;
      background-color: #FFFFFF;
      z-index: 2;
      transition: transform .5s;
      transform: translateX(0);
      border-left: 2px solid black;
      border-bottom: 2px solid black;
    }
    .menu.open {
      transform: translateX(100%);
    }
    .menuBtn {
      color: white;
      background-color: #7F31FF;
      font-weight: 900;
    }
    .menuLink {
      font-size: 20px;
      font-weight: 500;
      display: flex;
      justify-content: center;
      padding: 20px 0px;
      width: 100%;
      color: #590BD9;
    }
    .menu div:hover {
      opacity: 0.7;
      cursor: pointer;
    }
    .menu div:nth-child(2) {
      border-top: 1px solid #505050;
      border-bottom: 1px solid #505050;
    }
    .menu div:nth-child(3) {
      border-bottom: 1px solid #505050;
    }
    .menuBtn {
      color: #FFFFFF;
      background-color: #7F31FF;
    }
  }
</style>