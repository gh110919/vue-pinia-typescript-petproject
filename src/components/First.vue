<script setup lang="ts">
import Socials from "./Socials.vue";
import Buttons from "./Buttons.vue";
</script>

<template>
  <section class="first">
    <div class="circle-2">
      <img src="../assets/circle-2.svg" alt="" />
    </div>
    <img class="guitarist" src="../assets/guitarist.png" alt="" />
    <div class="container">
      <div class="circle">
        <img src="../assets/circle-1.svg" alt="" />
      </div>
      <Socials></Socials>
      <div class="text">
        <h1 class="title"><span class="line"></span>Я Виктор</h1>
        <p class="subtitle">
          Репетитор игры на гитаре с семилетним опытом преподавания
        </p>
      </div>
      <Buttons></Buttons>
    </div>
  </section>
</template>

<style scoped>
.text {
  margin-bottom: 20px;
}
.container {
  margin-top: 140px;
  transform: translate(-41px, 2px);
  position: relative;
}

.circle {
  position: absolute;
  top: -13px;
  right: -42px;
  z-index: -1;
}

.guitarist {
  transform: translate(150px, -43px);
}

.first {
  width: 1440px;
  display: flex;
  flex-direction: row;
  position: relative;
}

.circle-2 {
  position: absolute;
  bottom: -84px;
  right: -99px;
  z-index: -1;
}

.title {
  /* Я Виктор */
  width: 353px;
  height: 88px;

  color: rgb(0, 0, 0);
  font-family: Montserrat;
  font-size: 72px;
  font-weight: 600;
  line-height: 88px;
  letter-spacing: 0%;
  text-align: left;
  position: relative;
}

.line {
  position: absolute;
  bottom: 10px;
  left: 1px;
  width: 65px;
  height: 1px;
  background-color: black;
}

.subtitle {
  transform: translate(0px, -4px);
  /* Репетитор игры на гитаре с семилетним опытом преподавания */
  width: 353px;
  height: 40px;

  color: rgb(0, 0, 0);
  font-family: Montserrat;
  font-size: 16px;
  font-weight: 400;
  line-height: 20px;
  letter-spacing: 0%;
  text-align: left;
}
</style>
