<template>
  <div class="bg-dark">
    <div class="container">
      <nav class="container navbar navbar-expand-lg" data-bs-theme="dark">
        <div class="container-fluid">
          <router-link to="/" class="navbar-brand">InDriver</router-link>
          <button
            class="navbar-toggler"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#navbarScroll"
            aria-controls="navbarScroll"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarScroll">
            <ul
              class="navbar-nav me-auto my-2 my-lg-0 navbar-nav-scroll"
              style="--bs-scroll-height: 200px"
            >
              <li class="nav-item">
                <router-link to="/" class="nav-link btn">Inicio</router-link>
              </li>
              <li class="nav-item">
                <router-link to="/about" class="nav-link btn"
                  >Nosotros</router-link
                >
              </li>
              <li class="nav-item">
                <router-link to="/upload" class="nav-link btn"
                  >Mi Musica</router-link
                >
              </li>
              <li class="nav-item">
                <router-link to="/contact" class="nav-link btn"
                  >Contacto</router-link
                >
              </li>
            </ul>
          </div>
        </div>
      </nav>
    </div>
  </div>
</template>
