<script setup lang="ts"></script>

<template>
  <div class="wrapper">
    <button class="button">
      <p class="button__text">Забронировать урок</p>
    </button>
    <a class="questions" href="">
      <img src="../assets/chat.svg" alt="" />
      <p class="question">Есть вопросы?</p>
    </a>
  </div>
</template>

<style scoped>
.button {
  /* Rectangle 1 */
  width: 200px;
  height: 60px;

  border: none;
  border-radius: 100px;
  box-shadow: 0px 4px 4px 0px rgba(0, 0, 0, 0.25);
  background: rgb(242, 139, 100);

  display: flex;
  justify-content: center;
  align-items: center;
}

.button__text {
  transform: translate(-2px, 1px);
  /* Забронировать урок */
  width: 152px;
  height: 38px;

  color: rgb(255, 255, 255);
  font-family: Montserrat;
  font-size: 18px;
  font-weight: 600;
  line-height: 105.19%;
  letter-spacing: 0%;
  text-align: center;
}
.wrapper {
  transform: translate(0px, -5px);
  display: flex;
  gap: 32px;
}

.questions {
  transform: translate(0px, -4px);
  display: flex;
  gap: 12px;
  justify-content: center;
  align-items: center;
}

.question {
  transform: translate(0px, 1px);
  width: 82px;
  color: rgb(0, 0, 0);
  font-family: Montserrat;
  font-size: 16px;
  font-weight: 300;
  line-height: 105.19%;
  letter-spacing: 0%;
  text-align: left;
}
</style>
