<script setup>
import Form from './components/Form.vue';
import FormPass from './components/FormPass.vue';
import FormAd from './components/FormAd.vue';
</script>

<template>
  <h1>Заполните форму</h1>
    <div class="divApp">
      <Form/>
      <!-- <FormAd/> -->
      <!-- <FormPass/> -->
    </div>


</template>

<style scoped>

.divApp{
  display: flex;
  flex-direction: row
}
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
