<template>
  <!-- // 글목록들 채워 넣을곳 -->
    <div>
        <h5>{{블로그글}}</h5>
        <p>블로그 글 날짜</p>
    </div>
    <div>
        <h5>{{블로그글[1].title}}</h5>
        <p>{{블로그글[1].date}}</p>
    </div>
</template>

<script>
export default {
    props : {
        블로그글 : Array,
    }

}
</script>

<style>

</style>