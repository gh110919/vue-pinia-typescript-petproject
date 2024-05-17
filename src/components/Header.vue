<script setup lang="ts"></script>

<template>
  <header class="header">
    <img class="header__logo" src="../assets/logo.svg" alt="">
    <div class="header__links">
      <a class="header__link" href="">Обо мне</a>
      <a class="header__link" href="">Занятия</a>
      <a class="header__link" href="">Запись</a>
    </div>
  </header>
</template>

<style scoped>
.header {
  margin-top: 16px;
  width: 1098px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

.header__logo{
  transform: translate(2px, 0px);
}

.header__links {
  transform: translate(0px, -3px);
  width: 363px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.header__link {
  color: rgb(0, 0, 0);
  font-family: Montserrat;
  font-size: 18px;
  font-weight: 600;
  line-height: 22px;
  letter-spacing: 0%;
  text-align: left;
}
</style>