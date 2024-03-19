<script setup></script>
<template>
  <section id="home-page">
    <div v-if="1 + 1 === 2" class="create-quizz">
      <h5>Você não criou nenhum <br />quizz ainda :(</h5>
      <button>Criar Quizz</button>
    </div>

    <div v-else class="all-quizzes">
      <div class="quizzes-header">
        <h3>Seus Quizzes</h3>
        <button>+</button>
      </div>

      <div class="cover-quizz">
        <span class="image-overlay"></span>
        <img
          src="https://tm.ibxk.com.br/2022/04/14/14130747357290.jpg"
          alt="Capa quizz"
        />
        <p>Acerte os personagens corretos dos Simpsons e prove seu amor</p>
      </div>
    </div>

    <div class="all-quizzes">
      <h3>Todos os Quizzes</h3>

      <div class="cover-quizz">
        <span class="image-overlay"></span>
        <img
          src="https://tm.ibxk.com.br/2022/04/14/14130747357290.jpg"
          alt="Capa quizz"
        />
        <p>Acerte os personagens corretos dos Simpsons e prove seu amor</p>
      </div>
    </div>
  </section>
</template>
<style lang="scss" scoped>
#home-page {
  margin: 70px;

  .create-quizz {
    border-radius: 5px;
    margin-bottom: 70px;
    height: 180px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    border: medium dashed #d4d4d4;

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
  }

  .quizzes-header {
    display: flex;
    align-items: center;
    margin-bottom: 10px;

    h3 {
      margin: 0;
    }

    button {
      background-color: #ec362d;
      border-radius: 50%;
      width: 30px;
      height: 30px;
      color: white;
      border: none;
      margin-left: 15px;
    }
  }

  .cover-quizz {
    position: relative;
    width: 340px;
    border-radius: 5px;
    overflow: hidden;

    img {
      max-width: 100%;
    }

    .image-overlay {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: linear-gradient(
        to top,
        rgba(0, 0, 0, 0.8) 0%,
        rgba(0, 0, 0, 0) 100%
      );
      mix-blend-mode: multiply;
    }

    p {
      position: absolute;
      max-width: 100%;
      text-align: center;
      bottom: 0;
      left: 0;
      padding: 10px;
      margin: 0;
      font-size: 19px;
      color: white;
    }
  }

  .all-quizzes {
    margin: 70px 0;

    h3 {
      font-size: 20px;
      font-weight: bold;
    }

    button {
      background-color: #ec362d;
      border-radius: 50%;
      width: 30px;
      height: 30px;
      color: white;
      border: none;
      margin-left: 15px;
    }
  }
}
</style>
