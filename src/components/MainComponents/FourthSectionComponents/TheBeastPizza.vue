<template>
    <section class="row">
        <div id="the-beast-pizza" class="col-12 position-relative d-flex flex-column align-items-center justify-content-center py-5">
            <!-- Box con testo -->
            <div id="pizza-slider" class="text-center">
                <span class="text-uppercase text-danger">chose your flavour</span>
                <h2 class="text-uppercase fs-1 mt-2 mb-4">
                    the beast pizza menu in town
                </h2>
                <p class="fs-5">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sint natus odio non iste voluptatem libero magnam, error repellendus dolorum et.</p>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name:'TheBeastPizza',

}
</script>

<style lang='scss' scoped>
    div#the-beast-pizza{
        height: 40vh;

        div#pizza-slider{
            width: 600px;

            p{
                font-weight: 300;
                color: #5a5a5a;
            }

            span{
                font-size: .8rem;
                letter-spacing: .2rem;
                font-weight: 500;
            }
        }
    }

</style>