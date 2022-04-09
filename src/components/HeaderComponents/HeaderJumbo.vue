<template>
    <section class="row">
        <div id="header-jumbo" class="col-12 d-flex align-items-center justify-content-center position-relative py-4">
            <img src="@/assets/img/h3-rev-img-6.png" alt="">
            
            <!-- PREV BTN -->
            <div class="circle-btn prev-btn rounded-circle text-danger position-absolute text-uppercase px-4 py-2">
                <span>p r e v</span>
            </div>
            
            <!-- NEXT BTN -->
            <div class="circle-btn next-btn rounded-circle text-danger position-absolute text-uppercase px-4 py-2">
                <span>n e x t</span>
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
        margin-top: 20vh;
        background-image: url('@/assets/img/h3-rev-img-5.png');
        background-size: 800px;
        background-position: center;
        background-repeat: no-repeat;

        img{
            width: 400px;
        }

        div.circle-btn{
            height: 85px;
            width: 85px;
            cursor: pointer;
            background-color: #f7f7f7;

            span{
                font-size: .8rem;
                font-weight: 600;
            }
        }

        div.prev-btn{
            top: 50%;
            left: -50px;
            transform: translate(0, -50%);
            transform: rotate(90deg);
        }

        div.next-btn{
            top: 50%;
            right: -50px;
            transform: translate(0, -50%);
            transform: rotate(-90deg);
        }
    }

</style>