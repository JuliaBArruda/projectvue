<!-- Navbar.vue -->
<template>
  <nav class="navbar sticky navbar-expand-lg navbar-light bg-light">
    <div class="container">
      <div class="col-md-3 ml-3 text-center">
        <router-link to="/">
          <img
            src="@/assets/img/logo.svg"
            alt="logo-subway"
            width="200"
            height="100"
            class="logo-hover"
          />
        </router-link>
      </div>
      <button
        class="navbar-toggler border-0 shadow-none"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNavDropdown"
        aria-controls="navbarNavDropdown"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="material-icons" style="font-size: 39px; color: black">
          menu_open
        </span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavDropdown">
        <ul class="navbar-nav me-5">
          <li class="nav-item">
            <a class="nav-link" href="#"> Home </a>
          </li>
          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              href="#"
              id="navbarDropdownMenuLink"
              role="button"
              data-bs-toggle="dropdown"
              aria-expanded="false"
            >
              Cardápio
            </a>
            <ul class="dropdown-menu" aria-labelledby="navbarDropdownMenuLink">
              <li>
                <router-link to="/paes" class="dropdown-item"
                  >Nossos Pães</router-link
                >
              </li>
              <li>
                <router-link to="/montar" class="dropdown-item"
                  >Como montar o Subway</router-link
                >
              </li>
              <li>
                <router-link to="/nutricionais" class="dropdown-item"
                  >Informações Nutricionais</router-link
                >
              </li>
            </ul>
          </li>
          <li class="nav-item">
            <a href="#" class="nav-link">Avalie o Subway</a>
          </li>
          <li class="nav-item">
            <a href="#" class="nav-link">Seja um Franqueado</a>
          </li>
        </ul>
        <div class="ms-auto">
          <a href="#" class="btn btn-white d-block d-md-inline-block"
            >Peça Já</a
          >
        </div>
      </div>
    </div>
  </nav>
</template>
  
    <script>
export default {
  name: "MainNavbar",
};
</script>
    
<style scoped>
.logo-hover:hover {
  transform: scale(1.05); /* Efeito de escala no hover */
  transition: transform 0.3s ease-in-out;
}

.material-icons {
  font-family: "Material Icons", sans-serif;
}

.btn-white {
  font-family: "Subway Sans Cond", sans-serif;
  background-color: #f3b304;
  color: #2c5c18;
  font-weight: 700;
  padding: 12px 30px;
  border-radius: 8px;
  transition: background-color 0.3s, color 0.3s;
}

.btn-white:hover {
  background-color: #2c5c18;
  color: #fff;
  box-shadow: 0px 0px 38px rgba(0, 0, 0, 0.12);
}

.navbar-nav li.nav-item a.nav-link,
li.nav-link {
  font-family: "Subway Sans Cond", sans-serif;
  color: rgb(110, 117, 88);
  font-size: 16px;
  line-height: 98.5%;
  font-weight: 600;
  margin-left: 40px; 
  margin-right: 35px;

}

.navbar-nav li.nav-item a.nav-link:hover,
.navbar-nav li.nav-item a.nav-link:focus,
li.nav-link:hover,
li.nav-link:focus {
  color: #2c5c18;
}
</style>
    