<script setup lang="ts">
import electro from "../assets/electro.png";
import acoustic from "../assets/acoustic.png";
import ukulele from "../assets/ukulele.png";
import cup from "../assets/cup.svg";
import reviews from "../assets/reviews.svg";
import trained from "../assets/trained.svg";
import hours from "../assets/hours.svg";

const guitarsArray = [
  {
    image: electro,
    text: "Электро гитара",
    color: "#E2E2E2",
    translate: "translate(-0px, 36px)",
  },
  {
    image: acoustic,
    text: "Акустическая гитара",
    color: "#F28B64",
    translate: "translate(-5px, 89px)",
  },
  {
    image: ukulele,
    text: "Укулеле гитара",
    color: "#5290EA",
    translate: "translate(-0px, 36px)",
  },
];

const studyArray = [
  {
    image: cup,
    title: "7",
    subtitle: "лет преподавания",
    translate: "translate(52px, 0px)",
  },
  {
    image: reviews,
    title: "276",
    subtitle: "Отзывов на\u00A05\u00A0звезд",
    translate: "translate(86px, 1px)",
  },
  {
    image: trained,
    title: "314",
    subtitle: "Студентов обученно",
    translate: "translate(76px, 0px)",
  },
  {
    image: hours,
    title: "2000",
    subtitle: "часов преподавания",
    translate: "translate(52px, 0px)",
  },
];
</script>

<template>
  <section class="second">
    <div>
      <h2 class="title"><span class="line"></span>Преподаю</h2>
      <ul class="list">
        <div class="circle-3">
          <img src="../assets/circle-3.svg" alt="" />
        </div>
        <li
          class="list__item"
          v-for="(e, i) in guitarsArray"
          :key="i"
          :style="{ backgroundColor: e.color }"
        >
          <div class="image">
            <img :src="e.image" :alt="e.text" />
          </div>
          <p class="text" :style="{ transform: e.translate }">{{ e.text }}</p>
        </li>
        <div class="circle-4">
          <img src="../assets/circle-4.svg" alt="" />
        </div>
      </ul>
      <ul class="study__list">
        <li
          class="study__list-item"
          v-for="(e, i) in studyArray"
          :key="i"
          :style="{ transform: e.translate }"
        >
          <div class="study__image">
            <img :src="e.image" :alt="e.subtitle" />
          </div>
          <div>
            <h3 class="study__title">{{ e.title }}</h3>
            <p class="study__subtitle">{{ e.subtitle }}</p>
          </div>
        </li>
      </ul>
    </div>
  </section>
</template>

<style scoped>
.study__title {
  width: 30px;
  height: 48px;

  color: rgb(0, 0, 0);
  font-family: Montserrat;
  font-size: 48px;
  font-weight: 600;
  line-height: 59px;
  letter-spacing: 0%;
  text-align: left;
  transform: translate(0px,-6px)
}
.study__subtitle {
  width: 139px;
  height: 44px;

  color: rgb(0, 0, 0);
  font-family: Montserrat;
  font-size: 18px;
  font-weight: 400;
  line-height: 22px;
  letter-spacing: 0%;
  text-align: left;
}
.study__list-item {
  display: flex;
  gap: 20px;
  width: min-content;
}
.study_image {
  width: min-content;
}
.study__list {
  width: 1035px;
  margin-top: 34px;
  display: flex;
  justify-content: space-between;
}
.text {
  rotate: 90deg;

  color: rgb(0, 0, 0);
  font-family: Montserrat;
  font-size: 36px;
  font-weight: 600;
  line-height: 44px;
  text-align: center;
}

.title {
  font-family: Montserrat;
  font-size: 72px;
  font-weight: 600;
  line-height: 87.77px;
  margin-bottom: 40px;
  margin-top: 32px;
  position: relative;
}

.line {
  position: absolute;
  bottom: 0px;
  left: 6px;
  width: 94px;
  height: 1px;
  background-color: black;
}

.image {
  width: 197px;
  height: 337px;
  transform: translate(0px, 14px);
}

.list {
  display: flex;
  gap: 30px;
  position: relative;
  z-index: 1;
}

.circle-3 {
  position: absolute;
  top: -93px;
  right: -53px;
  z-index: -1;
}

.circle-4 {
  position: absolute;
  bottom: -42px;
  left: -74px;
  z-index: -1;
}

.list__item {
  width: 360px;
  height: 360px;
  border-radius: 10px;
  box-shadow: 0px 4px 4px 0px rgba(0, 0, 0, 0.25);

  display: flex;
  align-items: center;
  gap: 25px;
}

.second {
  margin-top: -45px;
  width: 1440px;
  height: 700px;
  background-color: white;
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
