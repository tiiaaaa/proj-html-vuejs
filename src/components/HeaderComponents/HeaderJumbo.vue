<template>
    <section class="row">
        <div id="header-jumbo" class="col-12 text-center position-relative py-4">
            <img src="@/assets/img/h3-rev-img-6.png" alt="">

            <div class="circle-btn rounded-circle text-danger position-absolute text-uppercase p-2">
                prev
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
        height: 50vh;
        margin-top: 15vh;
        background-image: url('@/assets/img/h3-rev-img-5.png');
        background-size: 600px;
        background-position: center;
        background-repeat: no-repeat;

        img{
            width: 250px;
        }

        div.circle-btn{
            height: 60px;
            width: 60px;
            top: 50%;
            left: -30px;
            transform: translate(0, -50%);
            transform: rotate(90deg);
            font-size: .7rem;
            font-weight: 600;
            cursor: pointer;
            background-color: #f7f7f7;
        }
    }

</style>