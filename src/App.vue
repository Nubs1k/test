<script setup>

import {defineComponent} from "vue";
import Header from "./comonents/Header.vue";
import List from "./comonents/List.vue";
import AddNewSections from "./comonents/AddNewSections.vue";

const todos=[
  {id:0,title:"1"},
  {id:1,title:"2"},
  {id:2,title:"3"},
  {id:3,title:"4"},
  {id:4,title:"5"},
]
</script>
<template>
<div class = "content">
<Header></Header>
  <List :todos="todos"></List>
  <AddNewSections></AddNewSections>
</div>
</template>
<style scoped>
.content{
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: space-between;
  height: 100vh;
  font-size: 50px;
}
.list-item{
  border:5px solid green;
  padding:1rem;
  border-radius: 30px;
}
.list >*:not(:last-child){
  margin-bottom: 10px;
}
.button{
  background: aqua;
  font-size: 50px;
  border: 5px solid red;
  padding: 25px;
  border-radius: 50px;
}
.button-container{
  border: 10px dotted blue;
  border-bottom: none;
  padding: 30px;
  border-radius: 40px 40px 0 0;
}
</style>