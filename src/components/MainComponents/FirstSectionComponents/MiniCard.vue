<template>
    <section class="row py-2">
        <div class="mini-card col-12 col-sm-6 col-md-3 px-1 mb-2">
            <img src="@/assets/img/h3-img-1.jpg" alt="">
        </div>
        <div class="mini-card col-12 col-sm-6 col-md-3 px-1 mb-2">
            <img src="@/assets/img/h3-img-2.jpg" alt="">
        </div>
        <div class="mini-card col-12 col-sm-6 col-md-3 px-1 mb-2">
            <img src="@/assets/img/h3-img-3.jpg" alt="">
        </div>
        <div class="mini-card col-12 col-sm-6 col-md-3 px-1 mb-2">
            <img src="@/assets/img/h3-img-4.jpg" alt="">
        </div>
    </section>
</template>

<script>
export default {
    name: 'MiniCard',
}
</script>

<style lang='scss' scoped>
    div.mini-card{
            height: 260px;

            img{
                width: 100%;
                height: 100%;
                object-fit: cover;
                object-position: center;
            }
        }

</style>