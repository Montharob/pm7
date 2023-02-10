<script setup>
import news from "../json/news.json";
</script>

<template>
  <div class="content">
    <hr />

    <h5>ข่าวสารล่าสุด</h5>
    <article>
      <table>
        <tr>
          <th>วันที่</th>
          <th>หัวข้อข่าว</th>
        </tr>

        <tr v-for="news_content in news" :key="news_content.newsId">
          <td style="text-align: left">{{ news_content.News_Date }}</td>
          <td style="text-align: left">
            <a :href="news_content.News_links">{{ news_content.News_Title }}</a>
          </td>
        </tr>
      </table>
    </article>
  </div>
</template>
<style scoped>
.content {
  margin-top: 1em;
  margin-bottom: 1em;
}
.m-0 {
  margin: unset;
}

.color-gray {
  color: rgb(44, 79, 39);
}
</style>
