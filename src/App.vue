<script setup>
//import "@/assets/css/pico.min.css";
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <main class="container">
    <img src="../src/img/pokmrfds.png" alt="banner" />
    <header class="header-margin">
      <nav>
        <RouterLink to="/">หน้าแรก</RouterLink>
        <RouterLink to="/courses">รายวิชา</RouterLink>
        <RouterLink to="/enrollments">ลงทะเบียนเรียน</RouterLink>
        <RouterLink to="/mycourse">วิชาที่ฉันลงทะเบียน</RouterLink>
      </nav>
    </header>

    <RouterView />
  </main>
</template>

<style scoped>
.header-margin {
  padding-top: 0.8em;
  padding-bottom: 0.8em;
}

nav > a {
  padding-left: 0.5em;
  padding-right: 0.5em;
}
</style>
