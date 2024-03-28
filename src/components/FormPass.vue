<script setup>

</script>
<!-- 
  <input v-model="message" placeholder="отредактируй меня">
<p>Введённое сообщение: {{ message }}</p>
 -->
<template>
  <div
  class="DivName">
  <h3>Паспортные данные</h3>
    Введите тип документа*
    <select 
    class="inputT" 
    >
      <option>Паспорт</option>
      <option>Свидетельство о рождении</option>
      <option>Вод. удостверение</option>
    </select>

    Введите тип документа
    <input class="inputT" placeholder="Введите серию"/>
    Введите номер
    <input class="inputT" placeholder="Введите номер"/>
    Введите кем выдан
    <input class="inputT" placeholder="Введите кем выдан"/>
    Введите дату выдачи*
    <input class="inputT" placeholder="Введите дату выдачи"/>
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