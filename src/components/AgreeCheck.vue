<template>
<div class="agree-wrap">
  <span class="chk_wrap">
    <input type="checkbox" id="chk" v-model="checked">
  <label for="chk"></label>
  </span>
  <span class="txt">모든 약관 내용에 동의 합니다.</span>
</div>
</template>
<script>
  export default{
    data() {
  		return {
  			checked: []
  		}
	 }
  }
</script>
<style>
.agree-wrap{vertical-align:middle;line-height:26px;}
.agree-wrap span{display:inline-block;font-size:13px;line-height:6px;}
.agree-wrap .txt{padding-left:15px;}
.chk_wrap {position:relative;}
.chk_wrap label {position:absolute;top:0;left:0;width:26px;height:26px;background-color:#fff;border:2px solid #e9e9e9;border-radius:50%;box-sizing:border-box;cursor:pointer;}
.chk_wrap label:after{position:absolute;left:6px;top:7px;content: "";width:9px;height:4px;border:2px solid #e9e9e9;border-right:none;border-top:none;transform:rotate(-45deg);}
.chk_wrap input[type="checkbox"]{visibility:hidden;}
.chk_wrap input[type="checkbox"]:checked + label{background-color:#ffdf00;border-color:#ffdf00;}
.chk_wrap input[type="checkbox"]:checked + label:after{border-color:#000;}
</style>
