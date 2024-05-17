<script setup lang="ts">
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";
import { useCounterStore } from "./stores/counter";

const counter = useCounterStore();

setInterval(() => {
  counter.increment();
  console.log(counter.count);
}, 10000);

</script>

<template>
  <div class="content">
    <Header></Header>
    <Main></Main>
    <Footer></Footer>
  </div>
</template>

<style scoped>
.content {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 1440px;
  overflow: hidden;
}
</style>
