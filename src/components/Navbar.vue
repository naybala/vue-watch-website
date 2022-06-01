<template>
  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg py-3 fixed-top bg-light">
    <div class="container">
      <img
        src="https://www.amazfit.com/static/version1653631126/frontend/Born/amazfit01/en_US/images/logo.png"
        class="img-fluid"
        alt=""
      />
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navmenu"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navmenu">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item">
            <a href="#learn" class="nav-link">Watch Gallery</a>
          </li>
          <li class="nav-item">
            <a href="#questions" class="nav-link">Questions</a>
          </li>
          <li class="nav-item">
            <a href="#town" class="nav-link">Avaliable Shops</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
  <br /><br /><br />
</template>

<script></script>

<style scoped>
nav {
  z-index: 100;
}
a {
  transform: translateY(0);
  transition: 0.3s;
}

a:hover {
  border-radius: 0.5rem;
  transform: translateY(-10px);
  box-shadow: 3px 3px 10px rgb(204, 202, 202);
  transition: 0.3s;
}
</style>
