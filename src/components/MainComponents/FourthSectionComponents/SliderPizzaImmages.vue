<template>
    <section class="row">
        <div id="pizza-menu-slider">
            <!-- Singola card che racchiude ogni pizza -->
            <div class="pizza-card">
                <div class="pizza-object">
                    <!-- immagine della pizza -->
                    <div class="pizza-immage"></div>
                    <!-- Testo del menu -->
                    <div class="pizza-description"></div>
                </div>

                <!-- Bottoni che diventano visibili una volta in hover sulla card -->
                <div class="pizza-btns">
                    <button class="btn btn-danger rounded-0 py-2 px-3">
                        <span class="text-uppercase">add to cart</span>
                    </button>
                    <button class="btn btn-light rounded-0 py-2 px-3">
                        <span class="text-uppercase">quick view</span>
                    </button>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name:'SliderPizzaImmages',

}
</script>

<style lang='scss' scoped>

    div#pizza-menu-slider{
        height: 40vh;

        div.pizza-card{
            width: 300px;
            height: 100%;
            background-color: red;
            
            div.pizza-btns{

                button{
                    width: calc(100% / 2);

                    span{
                        font-size: .8rem;
                    }
                }
            }
        }
    }

</style>