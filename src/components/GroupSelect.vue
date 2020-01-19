<template>
<div class="sel-info">
  <dl class="birth-list">
    <dt>생일을 알려주세요.</dt>
    <dd>
      <div class="sel-wrap year">
        <select v-model="selected[0]">
          <option value="2000년" selected>2000년</option>
          <option>1999년</option>
          <option>1998년</option>
          <option>1997년</option>
          <option>1996년</option>
          <option>1995년</option>
        </select>
      </div>
      <div class="sel-wrap">
        <select v-model="selected[1]">
          <option selected value="01월">01월</option>
          <option>02월</option>
          <option>03월</option>
          <option>04월</option>
          <option>05월</option>
        </select>
      </div>
      <div class="sel-wrap">
    <select v-model="selected[2]">
        <option selected value="01일">01일</option>
        <option>02일</option>
        <option>03일</option>
        <option>04일</option>
        <option>05일</option>
      </select>
    </div>
    </dd>
  </dl>
  <dl class="tel-info">
    <dt>연락처를 알려주세요.</dt>
    <dd>
      <div class="sel-wrap">
      <select v-model="selected[3]">
        <option selected value="010">010</option>
        <option>011</option>
        <option>017</option>
      </select>
      </div>
      <input v-model.number="tel" type="number" placeholder="'-' 를 빼고 입력해주세요"  v-model="txt_number">
      <a href="#">인증</a>
    </dd>
  </dl>
</div>
</template>
<script>
  export default{
    data () {
    	return {
      	selected: ["2000년","01월","01일","010"],
        txt_number: ''
      }
    }
  }
</script>
<style>
.sel-info {width:100%;}
.sel-info select {position:relative;width:100%;text-indent:5px;height:30px;box-shadow:none;background:none;border:none;background-image: none;-webkit-appearance: none;-moz-appearance: none;appearance:none;border-radius: 0px;color:#000;}
.sel-info select option{color:#000;border-color:#000;}/*모바일 옵션창은 system이여서 따로 신경쓰지 않았습니다*/
.sel-info dt{color:#000;font-size:13px;font-weight:bold;}
.sel-info dd{overflow:hidden;margin-top:10px;border-bottom:1px solid #e5e5e5;}
.sel-info .sel-wrap{position:relative;float:left;}
.sel-info .sel-wrap::before{content:"";position:absolute;top:10px;right:10px;display:block;box-sizing: border-box;height:5px;width:5px;border-style: solid;border-color: #9d9d9d;border-width: 0px 1px 1px 0px;transform:rotate(45deg);}
.birth-list .sel-wrap{width:30%;}
.birth-list .year{width:40%;}
.sel-info select:focus{outline: none;}
.tel-info{margin-top:15px;}
.tel-info .sel-wrap{position:relative;float:left;width:30%;}
.tel-info input{float:left;display:block;width:50%;height:26px;border:none;margin-bottom:0px;}
.tel-info a{float:right;display:block;width:15%;height:28px;border:1px solid #cfd0d4;box-sizing:border-box;border-radius:2px;color:#4f5054;text-align:center;line-height:26px;}

</style>
