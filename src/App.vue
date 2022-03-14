<template>

<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Vue로그</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
      <div class="navbar-nav">
        <a class="nav-link active" aria-current="page" href="#">Home</a>
        <a class="nav-link" href="#">피쳐</a>
        <a class="nav-link" href="#">가격</a>
      </div>
    </div>
  </div>
</nav>

<!--  3. 본문에서 사용한다 -->


<div class="intorduce">
   <h1>Vue 튜토리얼 블로그입니다 </h1>
   <p> - Vue 스터디중 </p>
   
</div>

<List :블로그글="블로그글" />

</template>

<script>
import List from './components/articleList.vue';  // 1. Import를 먼저 하고
import article from './assets/blogArticle.js';

export default {
  name: 'App',
  data(){
    return{
      블로그글 : article
    }
  },
  components: {
    List : List,  //2. 등록을 하고
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
