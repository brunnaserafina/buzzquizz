<script setup></script>
<template>
  <div class="create-quizz">
    <h5>Você não criou nenhum <br>quizz ainda :(</h5>
    <button>Criar Quizz</button>
  </div>
</template>
<style scoped>
.create-quizz {
  border-radius: 5px;
  margin-top: 70px;
  height: 180px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  border: medium dashed #d4d4d4;
}

h5 {
  color: #b9b9b9;
  font-size: 20px;
  font-family: "Roboto", sans-serif;
  text-align: center;
}

button {
  color: #ec362d;
  border: medium dashed #ec362d;
  border-radius: 50px;
  background-color: transparent;
  height: 40px;
  width: 150px;
  margin-top: 15px;
  font-size: 20px;
}
</style>
