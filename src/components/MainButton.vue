<template>
<div class="btn-wrap">
  <button v-on:click="addInfo">가입하기</button>
</div>
</template>
<script>
export default{

}
</script>
<style>
.btn-wrap{display:block;width:100%;background-color:#ffdf00;margin-top:50px;border:1px solid #fcd70d;border-radius:5px;text-align:center;cursor:pointer;}
.btn-wrap button{display:inline-block;height:48px;padding:0px 48px;background-color:#ffdf00;color:#1b1b1b;line-height:48px;font-size:18px;font-weight:bold;text-align:center;}
</style>
