<script setup>



</script>

<template>

  <div
  class="DivName">
  <h3>О себе</h3>
    Введите имя*
    <input class="inputT" placeholder="Введите Имя"/>
    Введите фамилию*
    <input class="inputT" placeholder="Введите фамилию"/>
    Введите отчество
    <input class="inputT" placeholder="Введите отчество"/>
    Введите дату рождения*
    <input class="inputT" placeholder="Введите дату рождения"/>
    Введите номер телефона*
    <input class="inputT" placeholder="Введите номер телефона"/>
    Введите пол
    <input class="inputT" placeholder="Введите пол"/>
    Введите группу клиента*
    <input class="inputT" placeholder="Введите группу клиента"/>
    Выберите лечащего врача
    <select 
    class="inputT" 
    >
      <option>Иванов</option>
      <option>Захаров</option>
      <option>Чернышева</option>
    </select>
    <div>
      Не отправлять смс
      <input class="inputT" type="checkbox"/>
    </div>
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
