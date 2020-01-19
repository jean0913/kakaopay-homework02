<template>
  <div id="app">
    <form  v-on:submit="sendPost" >
    <MainTitle></MainTitle>
    <InputList></InputList>
    <BaseTab></BaseTab>
    <GroupSelect></GroupSelect>
    <AgreeCheck></AgreeCheck>
    <MainButton></MainButton>
  </form>
  </div>
</template>

<script>
import MainTitle from './components/MainTitle.vue'
import InputList from './components/InputList.vue'
import BaseTab from './components/BaseTab.vue'
import GroupSelect from './components/GroupSelect.vue'
import AgreeCheck from './components/AgreeCheck.vue'
import MainButton from './components/MainButton.vue'

export default {
  components:{
    'MainTitle' : MainTitle,
    'InputList' : InputList,
    'BaseTab' : BaseTab,
    'GroupSelect' : GroupSelect,
    'AgreeCheck' : AgreeCheck,
    'MainButton' : MainButton
  },
  data:{
     id: "",
     pw: "",
     gender: "",
     birth:"",
     tel:"",
     agree:''
 },
 methods: {
     sendPost: function(event){
         
     }
 }
}
</script>
<style>
html, body, div, span, h1, h2, h3, h4, h5, h6, p, blockquote, pre, a, abbr, acronym, address, big, cite, code, img, ins, kbd, q, s, samp, small, strike, strong, dl, dt, dd, ol, ul, li, fieldset, form, label, legend, table, caption, tbody, tfoot, thead, tr, th, td, figure {margin:0;padding:0;border:0;outline:0;letter-spacing:normal;line-height:normal;}
body{position:relative;-webkit-text-size-adjust:none;word-wrap:break-word;word-break:break-all;}
a{text-decoration:none;}
ul, ol, li{list-style-type:none;}
button{padding:0;cursor:pointer;outline:none;-webkit-text-size-adjust:none;border:none;}
button:focus {outline: none;}
body,th,td,input,select,textarea,button{font-size:12px;line-height:1.5;font-family:'Noto Sans KR','돋음',dotum,sans-serif;color:#1E1E1E;}
body{padding:0px 15px 30px 15px;}
.sel-info{margin-top:30px;}
.tab-list{margin-top:30px;}
.agree-wrap{margin-top:10px;}
.btn-wrap{margin-top:50px;}
</style>
