<template>
  <section class="p-5 p-lg-0 pt-lg-5 text-center text-sm-start" data-aos="fade-down">
    <div class="leftShowCase-1" @click="leftUp">
      <div class="container-left"></div>
    </div>
    <div class="leftShowCase-2" @click="leftDown">
      <div class="container-left"></div>
    </div>

    <div class="rightShowCase-1" @click="rightUp">
      <div class="container-right"></div>
    </div>
    <div class="rightShowCase-2" @click="rightDown">
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

<script>
export default {
  methods: {
    rightUp() {
      const rightCilckUp = document.querySelector(".rightShowCase-1");
      if (rightCilckUp.classList.contains("isOpened")) {
        rightCilckUp.classList.remove("changeUp2");
        rightCilckUp.classList.remove("isOpened");
      } else {
        rightCilckUp.classList.add("changeUp2");
        rightCilckUp.classList.add("isOpened");
      }
    },
    rightDown() {
      const rightClickDown = document.querySelector(".rightShowCase-2");
      if (rightClickDown.classList.contains("isOpened")) {
        rightClickDown.classList.remove("changeDown2");
        rightClickDown.classList.remove("isOpened");
      } else {
        rightClickDown.classList.add("changeDown2");
        rightClickDown.classList.add("isOpened");
      }
    },
    leftUp() {
      const leftClickUp = document.querySelector(".leftShowCase-1");
      if (leftClickUp.classList.contains("isOpened")) {
        leftClickUp.classList.remove("changeUp1");
        leftClickUp.classList.remove("isOpened");
      } else {
        leftClickUp.classList.add("changeUp1");
        leftClickUp.classList.add("isOpened");
      }
    },
    leftDown() {
      const leftClickDown = document.querySelector(".leftShowCase-2");
      if (leftClickDown.classList.contains("isOpened")) {
        leftClickDown.classList.remove("changeUp1");
        leftClickDown.classList.remove("isOpened");
      } else {
        leftClickDown.classList.add("changeUp1");
        leftClickDown.classList.add("isOpened");
      }
    },
  },
};
</script>

<style scoped>
.leftShowCase-1 {
  transition: all 0.3s;
  position: absolute;
  left: -5rem;
  transform: rotate(-40deg);
}

.leftShowCase-2 {
  transition: all 0.3s;
  position: absolute;
  left: -5rem;
  bottom: 1rem;
  transform: rotate(-40deg);
}

.rightShowCase-1 {
  transition: all 0.3s;
  position: absolute;
  right: -5rem;
  transform: rotate(40deg);
}

.rightShowCase-2 {
  transition: all 0.3s;
  position: absolute;
  right: -5rem;
  bottom: 1rem;
  transform: rotate(40deg);
}
.container-right {
  cursor: pointer;
  width: 350px;
  height: 100px;
  background-color: #6c63ff;
  border-top-left-radius: 5rem;
  border-bottom-left-radius: 5rem;
}

.changeUp1 {
  transition: all 0.3s;
  transform: rotate(40deg);
}
.changeDown1 {
  transition: all 0.3s;
  transform: rotate(40deg);
}
.changeUp2 {
  transition: all 0.3s;
  transform: rotate(-40deg);
}
.changeDown2 {
  transition: all 0.3s;
  transform: rotate(-40deg);
}

.container-left {
  cursor: pointer;
  width: 350px;
  height: 100px;
  background-color: #6c63ff;
  border-top-right-radius: 5rem;
  border-bottom-right-radius: 5rem;
}

button {
  transform: translateY(0);
  transition: 0.3s;
}

button:hover {
  transform: translateY(-10px);
  box-shadow: 3px 3px 10px black;
  transition: 0.3s;
}

@media (max-width: 1100px) {
  .container-left,
  .container-right {
    display: none;
  }
}
</style>
