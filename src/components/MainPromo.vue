<template>
    <div class="col-md-6">
      <div class="promo-card text-center p-4">
        <div class="img-container">
          <img :src="imgSrc" :alt="title" class="img-fluid rounded">
        </div>
        <h2 class="mt-3 mb-2 custom-h2 negrito">{{ title }}</h2>
        <p class="mb-4 custom-p">{{ description }}</p>
        <button type="button" class="btn btn-success custom-button2 botao-negrito">
          Saiba Mais
        </button>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "PromoCard",
    props: {
      imgSrc: String,
      title: String,
      description: String,
    },
  };
  </script>
  
  <style scoped>
  @font-face {
  font-family: "Subway Sans Cond";
  src: url('@/fonts/SubwaySansCond-Bold.ttf') format('truetype');
  }

.custom-h2 {
  font-family: 'Subway Sans Cond', sans-serif;
  font-size: 36px;
  font-weight: 900;
  line-height: 40px;
  color: #05481f;
  background-color: #ffffff;
  text-align: left;
}

.custom-p {
    text-align: left;
    font-family: 'Roboto', sans-serif;
    font-size: 16px;
    font-weight: 500;
    line-height: 24px;
    word-spacing: 0px;
    background-color: #ffffff;
    background-position: 0% 0%;
    color: #05481f;
    margin: 8px 0 0;
}

.custom-button2 {
    font-family: "Subway Sans Cond", sans-serif;
    font-size: 20px;
    font-weight: 50;
    background-color: #048c3c;
    color: #ffffff;
}
.custom-button2:hover {
    background-color: #f2b304;
    color: #192719;
    box-shadow: 0px 0px 38px rgba(0, 0, 0, 0.12, );
}
  </style>
  