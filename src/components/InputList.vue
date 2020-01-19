<template>
  <ul class="input-list">
    <li><input type="text" placeholder="아이디" v-model="ID"></li>
    <li><input type="password" placeholder="비밀번호" v-model="PW"></li>
  </ul>
</template>
<script>
  export default{
    data(){
      return{
        ID:'',
        PW:''
      }
    }
  }
</script>
<style>
.input-list li{margin-top:5px;}
.input-list li:first-child{margin-top:0px;}
input[type="text"],input[type="password"]{width:100%;height:40px;border:1px solid #929197;color:#000;text-indent:10px;font-size:13px;}
</style>
