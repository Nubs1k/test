<template>
  <div class ="button-container">
    <button class="button">Добавить дело</button>
  </div>
</template>

<script>
export default {
  setup() {


    return {}
  }
}
</script>

<style  scoped>
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