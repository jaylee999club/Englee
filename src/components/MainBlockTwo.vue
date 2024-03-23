<template>
  <div class="block">
    <div class="blockOne">
        <img class="flagImg" src="../assets/usa.png">
        <div class="textBlock textBlockOne"><p class="text">Улучши свой английский</p><p class="text">Улучши свою память</p></div>
    </div>
    <div class="blockTwo">
        <div class="textBlock textBlockTwo"><p class="text">Улучши словарный запас</p><p class="text">Улучши свою жизнь</p></div>
        <img class="flagImg" src="../assets/england.png">
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
    .block {
        margin-top: 450px;
        display: flex;
        flex-direction: column;
    }
    .blockOne, .blockTwo {
        display: flex;
    }
    .blockOne {
        margin-bottom: 41px;
    }
    .text {
        font-weight: 700;
        font-size: 48px;
        color: #590BD9;
    }
    .textBlockOne {
        padding-left: 95px;
    }
    .textBlockTwo {
        padding-right: 95px;
    }
    .textBlock {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        margin: 30px 0px;
    }
    @media (max-width: 1150px) {
        .block {
            margin-top: 250px;
        }
        .flagImg {
            width: 212px;
            height: 161px;
        }
        .text {
            font-size: 32px;
        }
        .textBlockOne {
            padding-left: 65px;
        }
        .textBlockTwo {
            padding-right: 65px;
        }
        .textBlock {
            margin: 20px 0px;
        }
    }
    @media (max-width: 730px) {
        .block {
            margin-top: 250px;
        }
        .flagImg {
            width: 124px;
            height: 98px;
        }
        .text {
            font-size: 24px;
        }
        .textBlockOne {
            padding-left: 30px;
        }
        .textBlockTwo {
            padding-right: 30px;
        }
        .textBlock {
            margin: 5px 0px;
        }
    }
    @media (max-width: 450px) {
        .block {
            margin-top: 200px;
        }
        .blockOne {
            margin-bottom: 31px;
        }
        .flagImg {
            width: 104px;
            height: 78px;
        }
        .text {
            font-size: 19px;
        }
        .textBlockOne {
            padding-left: 25px;
        }
        .textBlockTwo {
            padding-right: 25px;
        }
        .textBlock {
            margin: 5px 0px;
        }
    }
</style>