<script setup>
</script>

<template>
  <header>
    <div class="bg-overlay"></div>
    <section>
      <div class="container">
        <nav class="navbar navbar-expand-lg ">
          <img src="../assets/img/menulogo.png" alt="">
          <ul class="navbar me-auto my-2 my-lg-0 navbar-nav-scroll gap-5 mx-5" style="--bs-scroll-height: 100px;">
              <li class="nav-item dropdown ms-color">
                <a class="nav-link dropdown-toggle ms-color" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  HOME
                </a>
                <ul class="dropdown-menu ms-color">
                  <li><a class="dropdown-item" href="#">About Us</a></li>
                  <li><hr class="dropdown-divider"></li>
                  <li><a class="dropdown-item" href="#">Matches</a></li>
                  <li><hr class="dropdown-divider"></li>
                  <li><a class="dropdown-item" href="#">Team</a></li>
                  <li><hr class="dropdown-divider"></li>
                  <li><a class="dropdown-item" href="#">Squad</a></li>
                </ul>
              </li>
              <li class="nav-item dropdown">
                <a class="nav-link dropdown-toggle ms-color text-white" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  PAGES
                </a>
                <ul class="dropdown-menu ms-color">
                  <li><a class="dropdown-item" href="#">About Us</a></li>
                  <li><hr class="dropdown-divider"></li>
                  <li><a class="dropdown-item" href="#">Matches</a></li>
                  <li><hr class="dropdown-divider"></li>
                  <li><a class="dropdown-item" href="#">Team</a></li>
                  <li><hr class="dropdown-divider"></li>
                  <li><a class="dropdown-item" href="#">Squad</a></li>
                </ul>
              </li>
              <li class="nav-item">
                <a class="nav-link  ms-color text-white" href="#">
                  TOURNAMENT
                </a>
              </li>
              <li class="nav-item dropdown">
                <a class="nav-link dropdown-toggle ms-color text-white" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  SHOP
                </a>
                <ul class="dropdown-menu ms-color">
                  <li><a class="dropdown-item" href="#">About Us</a></li>
                  <li><hr class="dropdown-divider"></li>
                  <li><a class="dropdown-item" href="#">Matches</a></li>
                  <li><hr class="dropdown-divider"></li>
                  <li><a class="dropdown-item" href="#">Team</a></li>
                  <li><hr class="dropdown-divider"></li>
                  <li><a class="dropdown-item" href="#">Squad</a></li>
                </ul>
              </li>
              <li class="nav-item dropdown">
                <a class="nav-link dropdown-toggle ms-color text-white" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  BLOG
                </a>
                <ul class="dropdown-menu ms-color">
                  <li><a class="dropdown-item" href="#">About Us</a></li>
                  <li><hr class="dropdown-divider"></li>
                  <li><a class="dropdown-item" href="#">Matches</a></li>
                  <li><hr class="dropdown-divider"></li>
                  <li><a class="dropdown-item" href="#">Team</a></li>
                  <li><hr class="dropdown-divider"></li>
                  <li><a class="dropdown-item" href="#">Squad</a></li>
                </ul>
              </li>
              <li class="nav-item">
                <a class="nav-link  ms-color text-white" href="#">
                  CONTACT
                </a>
              </li>
          </ul>
          
          <form class="d-flex" role="search">
            <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
            <button class="btn btn-outline-success" type="submit">Search</button>
          </form>
        </nav>
      </div>
    </section>
  </header> 
</template>

<style scoped>
li {
  list-style: none;
}
.ms-color {
  color: #05CC7C;
  list-style: none;
  font-weight:bold
}

header {
  position: relative;
  background-image: url("../assets/img/banner1.png");
  height: 45vw;
  width: 100%;
  background-size:cover;
  background-repeat: no-repeat;
}

.bg-overlay{
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(20, 20, 46, 0.5);
}
</style>
