<template>
  <div @click="top">
    <a href="#home #home" id="scroll-top">
      <i class="bi bi-arrow-up-circle-fill"></i>
    </a>
  </div>
</template>

<script>
window.onscroll = () => {
  if (window.scrollY > 0) {
    document.querySelector("#scroll-top").classList.add("active");
  } else {
    document.querySelector("#scroll-top").classList.remove("active");
  }
};
export default {
  methods: {
    top() {
      window.scroll({
        top: 0,
        behavior: "smooth",
      });
    },
  },
};
</script>

<style>
#scroll-top {
  position: fixed;
  top: -120%;
  right: 0.5rem;
  padding-left: 0.5rem;
  padding-right: 0.5rem;
  padding-bottom: 0.5rem;
  font-size: 2rem;
  color: whitesmoke;
  background-color: #0b5ed7;
  border-radius: 0.5rem;
  transition: 1s linear;
  z-index: 10;
}

#scroll-top.active {
  top: calc(100% - 4rem);
}

@media (max-width: 319px) and (min-width: 300px) {
  #scroll-top {
    font-size: 1rem;
    padding: 0.5rem 0.5rem;
  }
  #scroll-top.active {
    top: calc(100% - 7rem);
  }
}
@media (max-width: 550px) and (min-width: 320px) {
  #scroll-top {
    font-size: 1rem;
    padding: 0.5rem 0.5rem;
  }
  #scroll-top.active {
    top: calc(100% - 7rem);
  }
}
</style>
