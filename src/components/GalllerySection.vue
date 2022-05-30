<template>
  <div class="container text-center">
    <div class="gallery">
      <img
        src="https://images.unsplash.com/photo-1508685096489-7aacd43bd3b1?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MXx8c21hcnQlMjB3YXRjaHxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=500&q=60"
        alt=""
      />
      <img
        src="https://images.unsplash.com/photo-1434493789847-2f02dc6ca35d?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8N3x8c21hcnQlMjB3YXRjaHxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=500&q=60"
        alt=""
      />
      <img
        src="https://images.unsplash.com/photo-1517502474097-f9b30659dadb?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTB8fHNtYXJ0JTIwd2F0Y2h8ZW58MHx8MHx8&auto=format&fit=crop&w=500&q=60"
        alt=""
      />
      <img
        src="https://images.unsplash.com/photo-1555487505-8603a1a69755?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTZ8fHNtYXJ0JTIwd2F0Y2h8ZW58MHx8MHx8&auto=format&fit=crop&w=500&q=60"
        alt=""
      />
      <img
        src="https://images.unsplash.com/photo-1575125069494-6a0c5819d340?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MjB8fHNtYXJ0JTIwd2F0Y2h8ZW58MHx8MHx8&auto=format&fit=crop&w=500&q=60"
        alt=""
      />
      <img
        src="https://images.unsplash.com/photo-1596236100223-f3c656de3038?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTV8fHNtYXJ0JTIwd2F0Y2h8ZW58MHx8MHx8&auto=format&fit=crop&w=500&q=60"
        alt=""
      />
      <img
        src="https://images.unsplash.com/photo-1551816230-ef5deaed4a26?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8Nnx8c21hcnQlMjB3YXRjaHxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=500&q=60"
        alt=""
      />
      <img
        src="https://images.unsplash.com/photo-1579586337278-3befd40fd17a?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8NHx8c21hcnQlMjB3YXRjaHxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=500&q=60"
        alt=""
      />
    </div>
  </div>
  <br /><br />
</template>

<style lang="scss" scoped>
.gallery {
  display: grid;
  justify-content: center;
  grid-template-rows: repeat(5, 18vh);
  grid-template-columns: repeat(2, 45vw);
  transition: all 0.3s ease(gravity);
  border-radius: 2rem;
  padding: 0.25em;
  cursor: pointer;

  @media (min-width: 40em) {
    grid-template-rows: repeat(5, 18vh);
  }

  @media (min-width: 10em) and (orientation: landscape) {
    grid-template-rows: repeat(2, 45vh);
  }

  @media (min-width: 60em) {
    grid-template-columns: repeat(8, 8vw);
    grid-template-rows: 25vh;
  }
}

img {
  object-fit: cover;
  border-radius: 1rem;
  width: 100%;
  height: 100%;
  left: 0;
  top: 0;
  transition: all 0.3s;
  position: relative;
  box-shadow: 0 0 0 #0000;
  opacity: 0.67;
  //   filter: sepia(80%) hue-rotate(180deg);

  &:hover {
    opacity: 1;
    z-index: 1;
    box-shadow: 1em 1em 1em #0004;
    transition: all 0.3s;
    filter: sepia(0%) hue-rotate(0deg);
    border-radius: 5px;
    width: 200%;
    height: 200%;
    left: -50%;
    top: -50%;

    // @media (min-width: 10em) {
    //   width: 210%;
    //   height: 205%;
    // }
    @media (min-width: 60rem) and (orientation: landscape) {
      width: 300%;
      height: 250%;
      ~ img {
        left: 100px;
      }
    }
  }
}
</style>
