<template>
  <section id="learn" class="p-5">
    <div class="container">
      <div class="row align-items-center justify-content-between">
        <div class="col-md">
          <img
            src="https://www.xda-developers.com/files/2022/02/Amazfit-GTS-3-render.png"
            class="img-fluid rounded"
            alt=""
          />
        </div>
        <div class="col-md p-lg-0 pt-lg-5 text-center text-sm-start">
          <h2>Amaz Fit Gts-3 Pro</h2>
          <p class="lead">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Similique deleniti
            possimus magnam corporis ratione facere!
          </p>
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Cumque reiciendis
            eius autem eveniet mollitia, at asperiores suscipit quae similique laboriosam
            iste minus placeat odit velit quos, nulla architecto amet voluptates?
          </p>
          <div class="accordion accordion-flush">
            <div class="accordion-item">
              <h2 class="accordion-header">
                <button
                  class="accordion-button collapsed"
                  type="button"
                  data-bs-toggle="collapse"
                  data-bs-target="#readMore-Three"
                >
                  Read More
                </button>
              </h2>
              <div id="readMore-Three" class="accordion-collapse collapse">
                <div class="accordion-body">
                  <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Numquam
                    beatae fuga animi distinctio perspiciatis adipisci velit maiores totam
                    tempora accusamus modi explicabo accusantium consequatur, praesentium
                    rem quisquam molestias at quos vero. Officiis ad velit doloremque at.
                    Dignissimos praesentium necessitatibus natus corrupti cum consequatur
                    aliquam! Minima molestias iure quam distinctio velit.
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
img {
  cursor: pointer;
  transform: translateX(0px);
  transition: 0.3s;
}

img:hover {
  transform: translateX(-10px);
  box-shadow: 3px 3px 10px black;
  transition: 0.3s;
}
</style>
