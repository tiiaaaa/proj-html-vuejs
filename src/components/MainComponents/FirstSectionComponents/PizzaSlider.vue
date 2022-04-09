<template>
    <section class="row">
        <div id="pizza-box" class="col-12 position-relative d-flex flex-column align-items-center justify-content-center">
            <!-- Box con testo -->
            <div id="pizza-slider" class="text-center">
                <p class="text-uppercase fs-3 m-0">
                    “Forget the trendy pizza shops, This hidden spot makes the best New York-style pizza slice in naples”
                </p>
                <span class="text-uppercase text-danger">Washington Post 2018</span>
            </div>

            <!-- Contenitore puntini dello slider -->
            <div class="dots-wrapper d-flex mt-4">
                <div class="dot rounded-circle mx-1"></div>
                <div class="dot rounded-circle mx-1"></div>
                <div class="dot rounded-circle mx-1"></div>
            </div>
            
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
    name:'PizzaSlider',

}
</script>

<style lang='scss' scoped>
    div#pizza-box{
        height: 65vh;
        background-image: url('@/assets/img/h3-testimonials-bckgrnd.jpg');
        background-position: center;
        background-size: 2000px;
        background-repeat: no-repeat;
        background-color: #f6f7f2;

        div#pizza-slider{
            width: 900px;

            p{
                letter-spacing: .1rem;
                font-weight: 500;
            }

            span{
                font-size: .8rem;
                letter-spacing: .2rem;
                font-weight: 500;
            }
        }

        div.dots-wrapper{

            div.dot{
                height: 10px;
                width: 10px;
                cursor: pointer;
                background-color: orange;
            }
        }
    }
</style>