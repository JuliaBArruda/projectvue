<template>
    <footer class="bg-secondary bg-gradient bg-opacity-10 py-3">
      <div class="container">
        <div class="row">
          <div class="col-md-4 mb-4 footer-column">
            <img src="@/assets/img/logo.svg" alt="Subwaylogo" class="logo" />
          </div>
          <div class="col-md-4 text-center mb-4 footer-column">
            <div class="row">
              <router-link to="#">
                <a class="custom-a" to="#">Sobre Nós</a>
              </router-link>
              <a class="custom-a" to="#">App Subway Brasil (Beta)</a>
              <a class="custom-a" to="#">Avalie o Subway</a>
              <a class="custom-a" to="#">Subway Partners</a>
              <a class="custom-a" to="#">Trabalhe Conosco</a>
            </div>
          </div>
          <div class="col-md-4 text-center mb-4 footer-column">
            <div class="custom-text">
              <p>Acompanhe-nos nas redes sociais e fique por dentro das novidades!</p>
            </div>
            <a href="#" class="btn btn-primary btn-social me-3"><i class="fab fa-facebook"></i></a>
            <a href="#" class="btn btn-info btn-social me-3"><i class="fab fa-twitter"></i></a>
            <a href="#" class="btn btn-secondary btn-social me-3"><i class="fab fa-linkedin"></i></a>
            <a href="#" class="btn btn-danger btn-social me-3"><i class="fab fa-instagram"></i></a>
          </div>
          <div class="col-md-12 links-col d-flex justify-content-between mt-3 m-0">
            <a to="#" class="me-2">Código de Ética e Conduta SouthRock</a>
            <a to="#" class="me-2">Política de Privacidade</a>
            <a to="#" class="me-2">Termos de Uso</a>
            <a to="#" class="me-2">Política de Cookies</a>
          </div>
          <div class="row mt-3">
            <div class="col-md-12 text-center">
              <p>Todos os direitos reservados. &copy; 2023 </p>
            </div>
          </div>
        </div>
      </div>
    </footer>
  </template>
  
  <script>
  export default {
    name: "MainFooter",
  };
  </script>
  
  <style scoped>
  .footer-column {
    margin-bottom: 20px;
    
}

footer {
    padding: 20px 0;
    color: #234214;

}

footer * {
    font-weight: bold;
}


footer img.logo {
    max-width: 350px;
  
}

.footer-column a {
    text-decoration: none;
    
}
.custom-a {
    font-family: "Subway Sans Cond", sans-serif;
    color: #155417;
    font-size: 16px;
    font-weight: 500;
}
.custom-a:hover {
    color:#008938

}
footer a {
    font-family: "Subway Sans Cond", sans-serif;
    color: #155417;
    font-weight: 700;
    font-size: 20px;
    line-height: 24px;
}


footer a:hover {
    color: #048c3c;
}


footer .links-col a {
    display: block;
    margin-bottom: 5px;
}


footer .links-col a::before {
    margin-right: 5px;
}

.footer-column .btn-social {
    font-size: 24px;
    width: 40px;
    height: 40px;
    line-height: 40px;
    border-radius: 50%;
    
}

.footer-column p {
    font-family: "Subway Sans Cond", sans-serif;
    color: #2c5c18;
    font-weight: 700; 
    font-size: 20px; 
    line-height: 1.5; 
}

footer .me-2 {
    text-decoration: none;
    font-weight: 600
}

  </style>
  