<template>
    <div id="carouselExampleAutoplaying" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-inner">
            <div class="carousel-item active">
                <img src="../assets/bg.jpg" class="d-block w-100" alt="...">
                <div class="carousel-caption d-none d-md-block ">
                    <h5 class="text-start fw-bold">THIS IS A PLACE WHERE TECHNOLOGY & <br> CREATIVITY FUSED INTO DIGITAL CHEMISTRY </h5>
                </div>

            </div>
            <div class="carousel-item">
                <img src="../assets/about-bg.jpg" class="d-block w-100" alt="...">
                <div class="carousel-caption d-none d-md-block">
                    <h5 class="text-start fw-bold">WE DONT HAVE THE BEST BUT WE HAVE THE & <br> GREATEST TEAM </h5>
                </div>

            </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleAutoplaying"
            data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleAutoplaying"
            data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
        </button>
    </div>
</template>
  
<script>
export default {
    name: 'SliderVue',
}
</script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
  