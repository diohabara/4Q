<template>
  <div class="container bg-gray-100 h-screen m-auto max-w-600">
    <div class="p-4">
      <img class="logo" src="/logo.png" />
    </div>
    <div class="text-center">
      <h1 class="text-4xl">4Q 四択問題作成サイト</h1>
      <div class="text-xl">
        四択問題を簡単に作成して、SNSに広げてフォロワーに出題しよう！
      </div>
    </div>
    <div class="flex justify-center p-8">
      <TwitterButton @twitter-login="login" />
    </div>
    <div class="text-center text-2xl">
      <h2>遊び方</h2>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  methods: {
    login: function() {
      console.log("login");
    }
  }
});
</script>

<style scoped>
.max-w-600 {
  max-width: 750px;
}
.logo {
  width: 400px;
  height: 400px;
  margin: auto;
}
</style>
