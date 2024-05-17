<script setup lang="ts">
import Buttons from "./Buttons.vue";
</script>

<template>
  <section class="third">
    <div class="circle-5"><img src="../assets/circle-5.svg" alt="" /></div>
    <div class="title__box">
      <div class="circles">
        <img src="../assets/circles.svg" alt="" />
      </div>
      <h4 class="title"><span class="line"></span>Обучение</h4>
    </div>
    <div class="text__box">
      <h5 class="text__title"><span class="line-2"></span>Готовлю виртуозов</h5>
      <div class="text__wrapper">
        <p class="text">
          Равным образом рамки и место обучения кадров влечет за собой процесс
          внедрения и модернизации позиций, занимаемых участниками в отношении
          поставленных задач. Товарищи! реализация намеченных плановых заданий
          позволяет выполнять важные задания по разработке систем массового
          участия.
        </p>
        <p class="text">
          Повседневная практика показывает, что рамки и место обучения кадров
          позволяет оценить значение новых предложений. Не следует, однако
          забывать, что рамки и место обучения кадров влечет за собой процесс
          внедрения и модернизации систем массового участия.
        </p>
      </div>
      <div class="button__wrapper">
        <Buttons></Buttons>
      </div>
    </div>
  </section>
</template>

<style scoped>
.button__wrapper {
  transform: translate(-4px, 9px);
}
.text__wrapper {
  display: flex;
  flex-direction: column;
  gap: 23px;
}
.text {
  font-family: Montserrat;
  font-size: 18px;
  font-weight: 400;
  line-height: 21.94px;
  text-align: left;

  transform: translate(-3px, 0px);
}
.text__title {
  font-family: Montserrat;
  font-size: 72px;
  font-weight: 600;
  line-height: 64.73px;
  text-align: left;

  transform: translate(3px, 4px);
  position: relative;
}
.line-2 {
  position: absolute;
  top: 64px;
  left: 5px;
  width: 70px;
  height: 1px;
  background-color: black;
}
.text__box {
  width: 479px;
  display: flex;
  flex-direction: column;
  gap: 25px;

  transform: translate(0px, -3px);
}
.line {
  position: absolute;
  bottom: 11px;
  left: 1px;
  width: 70px;
  height: 1px;
  background-color: black;
}
.title {
  /* Обучение */
  width: 387px;
  height: 88px;

  color: rgb(0, 0, 0);
  font-family: Montserrat;
  font-size: 72px;
  font-weight: 600;
  line-height: 88px;
  letter-spacing: 0%;
  text-align: left;

  transform: translate(74px, 0);
  position: relative;
}
.circles {
  position: absolute;
  left: -4px;
  bottom: -4px;
  z-index: -1;
}
.title__box {
  width: 542px;
  height: 319px;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
}
.circle-5 {
  position: absolute;
  top: -121px;
  right: -94px;
}
.third {
  width: 1440px;
  height: 640px;
  display: flex;
  gap: 88px;
  justify-content: center;
  align-items: center;
  position: relative;
  overflow: hidden;
}
</style>
