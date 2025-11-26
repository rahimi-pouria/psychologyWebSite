<template>
  <div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="true">
    <div class="carousel-indicators">
      <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
      <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
      <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
    </div>
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="@/public/image/png/3fd237a0-b1a6-41e2-97d3-a78896ef170c-1764159381.png" class="d-block w-100" alt="...">
        <div class="overlay"></div>
      </div>
      <div class="carousel-item">
        <img src="@/public/image/png/823bd78c-22db-4fe8-99dd-e1c114479ed2.png" class="d-block w-100" alt="...">
        <div class="overlay"></div>
      </div>
      <div class="carousel-item">
        <img src="@/public/image/png/b7229745-5f2d-4542-8df6-e71bc25f3825-1764159279.png" class="d-block w-100" alt="...">
        <div class="overlay"></div>
      </div>
    </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Previous</span>
    </button>
    <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Next</span>
    </button>
  </div>
</template>

<script setup lang="ts">
</script>

<style scoped>
.carousel-inner {
  height: 130vh;
}

.carousel-item {
  position: relative;
}

.carousel-item img {
  height: 100%;
  object-fit: cover;
  object-position: center top;
  margin-top: -15rem;
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.3);
  z-index: 1;
}

span.carousel-control-prev-icon,
span.carousel-control-next-icon {
  border: 1px solid #fff;
  border-radius: 50%;
  padding: 25px;
  background-size: 50%;
  z-index: 2;
  position: relative;
}
</style>
