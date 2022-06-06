<template>
  <section id="learn" class="p-5 bg-dark text-light">
    <div class="container">
      <div class="row align-items-center justify-content-between">
        <div class="col-md p-lg-0 pt-lg-5 text-center text-sm-start">
          <h2>Amaz Fit T-Rex Pro</h2>
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
                  data-bs-target="#readMore-Two"
                >
                  Read More
                </button>
              </h2>
              <div id="readMore-Two" class="accordion-collapse collapse">
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
        <div class="col-md">
          <img
            src="https://m.media-amazon.com/images/I/71r-CE2J5ES._SL1500_.jpg"
            class="img-fluid rounded"
            alt=""
          />
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
  transform: translateX(10px);
  box-shadow: 3px 3px 10px rgb(161, 161, 161);
  transition: 0.3s;
}
</style>
