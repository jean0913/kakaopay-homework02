<template>
  <ul class="tab-list">
    <li><a href="#" v-on:click="gender==male">남자</a></li>
    <li class="on"><a href="#" v-on:click="gender==female" >여자</a></li>
  </ul>
</template>
<script>
  export default{
    data() {
        return {
          gender:''
        }
    }
  }
</script>
<style>
.tab-list{position:relative;width:100%;margin-top:30px;overflow:hidden;border:1px solid #929197;border-radius:7px;}
.tab-list::before{content:"";position:absolute;width:1px;height:40px;top:0px;left:50%;}
.tab-list li{float:left;width:50%;}
.tab-list li a{display:block;height:40px;background-color:#fff;color:#000;line-height:40px;text-align:center;font-size:13px;font-weight:bold;}
.tab-list li.on a{color:#fff;background-color:#2e303f;}
</style>
