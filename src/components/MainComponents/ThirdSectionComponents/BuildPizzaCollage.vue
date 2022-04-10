<template>
    <section id="build-pizza-collage" class="row">
        <div class="col-8 offset-2 d-flex align-items-center">
            <h2 class="text-uppercase text-white">
                Go Ahead and <br>
                Build Your<br>
                Own Pizza<br>
                We Won’t<br>
                Judge!
            </h2>

        </div>
    </section>
</template>

<script>
export default {
    name:'BuildPizzaCollage',

}
</script>

<style lang='scss' scoped>
    section#build-pizza-collage{
        height: 80vh;
        background-image: url('@/assets/img/h3-background-img.jpg');
        background-size: cover;
        background-position-x: right;
        background-repeat: no-repeat;

        h2{
            font-size: 4rem;
        }
    }

</style>