<script setup>

</script>

<template>
  <div
  class="DivName">
  <h3>Адрес</h3>
    Введите индекс
    <input class="inputT" placeholder="Введите индекс"/>
    Введите страну
    <input class="inputT" placeholder="Введите страну"/>
    Введите область
    <input class="inputT" placeholder="Введите область"/>
    Введите город*
    <input class="inputT" placeholder="Введите город"/>
    Введите улицу
    <input class="inputT" placeholder="Введите улицу"/>
    Введите дом
    <input class="inputT" placeholder="Введите дом"/>
  </div>
    
</template>

<style scoped>
.inputT{
  padding: 10px;
  margin: 10px;
}
.DivName{
  border: 4px, white;
  display: flex;
  flex-direction: column;
}
.pSt{
  background: #888;
  width: 30%;
}
.read-the-docs {
  color: #888;
}
</style>