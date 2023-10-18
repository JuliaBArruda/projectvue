<template>
  <div class="container mt-3 mb-5">
    <div id="carousel-item" class="carousel slide" data-bs-ride="carousel">
      <div class="carousel-indicators">
        <button
          type="button"
          data-bs-target="#carousel-item"
          data-bs-slide-to="0"
          class="active"
          aria-current="true"
          aria-label="Slide 1"
        ></button>
        <button
          type="button"
          data-bs-target="#carousel-item"
          data-bs-slide-to="1"
          aria-label="Slide 2"
        ></button>
        <button
          type="button"
          data-bs-target="#carousel-item"
          data-bs-slide-to="2"
          aria-label="Slide 3"
        ></button>
      </div>
      <div class="carousel-inner">
        <div class="carousel-item active c-item">
          <img
            src="@/assets/img/Banner1.jpg"
            class="d-block w-100 c-img"
            alt="Promo1"
          />
        </div>
        <div class="carousel-item c-item">
          <img
            src="@/assets/img/Banner2.jpg"
            class="d-block w-100 c-img"
            alt="Promo2"
          />
        </div>
        <div class="carousel-item c-item">
          <img
            src="@/assets/img/Banner3.jpg"
            class="d-block w-100 c-img"
            alt="Promo3"
          />
        </div>
      </div>
      <button
        class="carousel-control-prev"
        type="button"
        data-bs-target="#carousel-item"
        data-bs-slide="prev"
      >
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
      </button>
      <button
        class="carousel-control-next"
        type="button"
        data-bs-target="#carousel-item"
        data-bs-slide="next"
      >
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Next</span>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainCarousel",
};
</script>

<style scoped>
.c-item {
  height: 300px;
}

.c-img {
  height: 100%;
  object-fit: cover;
}
</style>