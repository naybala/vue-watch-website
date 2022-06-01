<template>
  <section class="p-5 p-lg-0 pt-lg-5 text-center text-sm-start" data-aos="fade-down">
    <div class="leftShowCase-1">
      <div class="container-left"></div>
    </div>
    <div class="leftShowCase-2">
      <div class="container-left"></div>
    </div>

    <div class="rightShowCase-1">
      <div class="container-right"></div>
    </div>
    <div class="rightShowCase-2">
      <div class="container-right"></div>
    </div>

    <div class="container">
      <div class="d-sm-flex align-items-center justify-content-between">
        <img
          class="img-fluid w-50 d-none d-sm-block"
          src="../assets/watch_showcase.svg"
          alt=""
        />
        <div>
          <h1><span class="text-dark"> Amaz-fit Global </span></h1>
          <p class="lead my-4">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Hic, neque. Lorem
            ipsum dolor sit amet consectetur adipisicing elit. Facere, maiores.
          </p>
          <a href="#learn">
            <button
              class="btn btn-dark btn-lg"
              data-bs-toggle="modal"
              data-bs-target="#enroll"
            >
              Discover More
            </button>
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<script></script>

<style scoped>
.leftShowCase-1 {
  position: absolute;
  left: -5rem;
  transform: rotate(-40deg);
}

.leftShowCase-2 {
  position: absolute;
  left: -5rem;
  bottom: 1rem;
  transform: rotate(-40deg);
}

.rightShowCase-1 {
  position: absolute;
  right: -5rem;
  transform: rotate(40deg);
}

.rightShowCase-2 {
  position: absolute;
  right: -5rem;
  bottom: 1rem;
  transform: rotate(40deg);
}
.container-right {
  width: 350px;
  height: 100px;
  background-color: #6c63ff;
  border-top-left-radius: 5rem;
  border-bottom-left-radius: 5rem;
}

.container-left {
  width: 350px;
  height: 100px;
  background-color: #6c63ff;
  border-top-right-radius: 5rem;
  border-bottom-right-radius: 5rem;
}

@media (max-width: 1100px) {
  .container-left,
  .container-right {
    display: none;
  }
}
</style>
