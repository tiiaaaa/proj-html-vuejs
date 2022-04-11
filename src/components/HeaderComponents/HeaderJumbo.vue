<template>
    <section class="row">
        <div id="header-jumbo" class="col-12 d-flex align-items-center justify-content-center position-relative py-4">
            <img src="@/assets/img/h3-rev-img-6.png" alt="">
            
            <!-- PREV BTN -->
            <div class="circle-btn prev-btn rounded-circle text-danger position-absolute text-uppercase px-4 py-2">
                <span>prev</span>
            </div>
            
            <!-- NEXT BTN -->
            <div class="circle-btn next-btn rounded-circle text-danger position-absolute text-uppercase px-4 py-2">
                <span>next</span>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'HeaderJumbo',

}
</script>

<style lang='scss' scoped>
    div#header-jumbo{
        height: 80vh;
        margin-top: 15vh;
        background-image: url('@/assets/img/h3-rev-img-5.png');
        background-size: 800px;
        background-position: center;
        background-repeat: no-repeat;

        img{
            width: 400px;
        }
    }

</style>