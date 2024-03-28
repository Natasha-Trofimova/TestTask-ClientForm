<script>
export default{
  data() {
    return{
      error: "",
      userName: "",
      userFamily: "",
      userSurname: "",
      userDatBirth: "",
      userNumbertell: "",
      userGender: "",
      userGroup: "",
      userDoctor: ""
    }
  },
  methods: {
    sendData(){
        // проверка ввода чтобы не пусто было имя
        if(this.userName == '') {
          this.error = 'имя не введено';
          return;
        }
        if(this.userFamily == '') {
          this.error = 'фамилия не введена';
          return;
        }
        if(this.userDatBirth == '') {
          this.error = 'дата рождения не указана';
          return;
        }
        if(this.userNumbertell == '') {
          this.error = 'не указан номер телефона';
          return;
        }
        if(this.userGroup == '') {
          this.error = 'не указана группа клиента';
          return;
        }
        this.error = '';


        this.users.push({
          name: this.userName,
          family: this.userFamily,
          surname: this.userSurname,
          datBirth: this.userDatBirth,
          numbertell: this.userNumbertell,
          gender: this.userGender,
          group: this.userGroup,
          doctor: this.userDoctor
        })
      }
  }
}


</script>

<template>
  <div
  class="DivName">
  <h3>О себе</h3>
  <p class="error">{{ error }}</p>

    Введите имя*
    <input v-model="userName" class="inputT" placeholder="Введите Имя"/>
    
    Введите фамилию*
    <input v-model="userFamily" class="inputT" placeholder="Введите фамилию"/>

    Введите отчество
    <input v-model="userSurname" class="inputT" placeholder="Введите отчество"/>
    
    Введите дату рождения*
    <input v-model="userDatBirth" class="inputT" placeholder="Введите дату рождения"/>
    
    Введите номер телефона*
    <input v-model="userNumbertell" class="inputT" placeholder="Введите номер телефона"/>
    
    Введите пол
    <input v-model="userGender" class="inputT" placeholder="Введите пол"/>
    
    Введите группу клиента*
    <input v-model="userGroup" class="inputT" placeholder="Введите группу клиента"/>
    
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

  <p class="error">{{ error }}</p>
    <button type="button" 
  @click="sendData()" 
  >
  Сохранить</button>
  </div>

  
</template>

<style scoped>
.inputT{
  padding: 10px;
  margin: 10px;
}
.error{
  color: red;
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
