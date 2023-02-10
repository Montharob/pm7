<template>
  <h3>รายวิชาทั้งหมด</h3>
  <hr />
  <table>
    <tr>
      <th>รหัสวิชา</th>
      <th>ชื่อวิชา</th>
    </tr>

    <tr v-for="(course, index) in courses" :key="index">
      <td style="text-align: left">{{ course.course_id }}</td>
      <td style="text-align: left">
        {{ course.course_name }}
      </td>
    </tr>
  </table>
</template>
<script setup>
import courses from "../json/cs_courses.json";
</script>
<style></style>
