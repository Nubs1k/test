<template>
  <div class ="list-container">
    <ul class ="list">
      <li v-for="todo in props.todos" class ="list-item">{{todo.title}}</li>
    </ul>
  </div>
</template>

<script setup>
const props= defineProps({
  todos:{
    type:Array,
    required:true
  }
})
</script>

<style  scoped>
.list-item{
  border:5px solid green;
  padding:1rem;
  border-radius: 30px;
}
.list >*:not(:last-child){
  margin-bottom: 10px;
}
</style>