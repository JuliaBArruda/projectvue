<template>
  <!-- Section -->
  <section id="services" class="services section-padding main-section mt-5">
    <div class="container">
      <div class="row">
        <div class="section-header text-center">
          <h2 class="mb-2 font-weight-bold custom-h2">Encontre uma loja</h2>
          <p class="custom-p mb-2 lead">
            Tenha uma experiência incrível! Digite seu endereço para encontrar
            lojas e promoções na sua região.
          </p>
          <button type="button" class="btn btn-light custom-button1 btn-lg mb-4 negrito">
            Encontre um SUBWAY®
          </button>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "MainSection",
};
</script>

<style scoped>
.custom-h2 {
  font-family: "Subway Sans Cond", sans-serif;
  font-size: 36px; /* Tornando responsivo */
  font-weight: 900;
  line-height: 1.2;
  color: #05481F;
  background-color: #ffffff;
  padding: 0vw; /* Ajuste conforme necessário */
  max-width: 100%;
  box-sizing: border-box;
}


.custom-p {
  font-family: 'Ariel', sans-serif;
  font-size: 20px; /* Ajuste conforme necessário */
  font-weight: 500;
  line-height: 28px;
  color: #545454;
  background-color: #ffffff;
  margin: 0 auto;
  margin-top: 20px;
  max-width: 576px;
  min-width: auto;
  text-align: center;
  word-wrap: break-word;
  hyphens: auto;
  box-sizing: border-box;
}



.main-section {
  margin-top: 1vw; 
}

.custom-button1 {
  margin-top: 20px;
  font-size: 16px;
  font-family: 'Subway San Cond', sans-serif;
  background-color: #008938;
  color: #ffffff;
  font-weight: 900;
  padding: 12px 10px;
  border-radius: 15px;
  transition: background-color 0.3s, color 0.3s;
}

.custom-button1:hover {
  background-color: #F2B700;
  color: #05481F;
  box-shadow: 0px 0px 38px rgba(0, 0, 0, 0.12);
}

</style>
