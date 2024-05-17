<script setup lang="ts">
import Socials from "./Socials.vue";
</script>

<template>
  <footer class="footer">
    <div class="neck">
      <img src="../assets/neck.png" alt="" />
    </div>
    <div>
      <h6 class="title"><span class="line"></span>Запишись на пробный урок</h6>
      <div class="socials__wrapper">
        <Socials></Socials>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.socials__wrapper {
  transform: translate(-20px, -45px);
}
.title {
  /* Запишись на пробный урок */
  width: 557px;
  height: 176px;

  font-family: Montserrat;
  font-size: 72px;
  font-weight: 600;
  line-height: 64.73px;
  text-align: left;

  margin-top: 50px;
  transform: translate(-9px, -10px);
  position: relative;
}
.line {
  position: absolute;
  top: 64px;
  left: 4px;
  width: 70px;
  height: 1px;
  background-color: black;
}
.neck {
  transform: translate(-5px, -10px);
}
.footer {
  width: 1440px;
  height: 274px;
  background-color: white;
  display: flex;
  gap: 97px;
}
</style>
