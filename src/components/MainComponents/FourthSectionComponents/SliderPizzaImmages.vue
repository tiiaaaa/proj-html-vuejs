<template>
    <section class="row">
        <div id="pizza-menu-slider" class="d-flex position-relative p-0">
            <!-- Singola card che racchiude ogni pizza -->
            <div class="pizza-card position-relative" v-for="(card, index) in PizzaCardList" :key="index">
                <div class="pizza-object p-3">
                    <!-- immagine della pizza -->
                    <div class="pizza-immage d-flex justify-content-center align-items-center">
                        <a href="#">
                            <img class="img-fluid" :src="card.url" :alt="card.type">
                        </a>
                    </div>
                    <!-- Testo del menu -->
                    <div class="pizza-description text-center py-3">
                        <h4 class="fs-4">
                            <a class="text-decoration-none text-uppercase" href="#">
                                {{card.type}}
                            </a>
                        </h4>

                        <span class="text-danger">{{card.price}}</span>
                    </div>
                </div>

                <!-- Bottoni che diventano visibili una volta in hover sulla card -->
                <div class="pizza-btns position-absolute">
                    <button class="function-btn btn btn-danger rounded-0 py-2 px-3">
                        <span class="text-uppercase">add to cart</span>
                    </button>
                    <button class="function-btn btn btn-light rounded-0 py-2 px-3">
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
    data: function(){
        return{
            PizzaCardList: [
                {
                    url: 'https://donpeppe.qodeinteractive.com/wp-content/uploads/2019/10/h3-product-img-1a.png',
                    type: 'Campagnola',
                    price: '$50.00 - $95.00'
                },

                {
                    url: 'https://donpeppe.qodeinteractive.com/wp-content/uploads/2019/10/h3-product-img-2a.png',
                    type: 'Fiori Di Zucca',
                    price: '$7.00 - $50.00'
                },

                {
                    url: 'https://donpeppe.qodeinteractive.com/wp-content/uploads/2019/10/h3-product-img-3a.png',
                    type: 'Bismark',
                    price: '$35.00 - $30.00'
                },

                {
                    url: 'https://donpeppe.qodeinteractive.com/wp-content/uploads/2019/10/h3-product-img-4a.png',
                    type: 'Pizza Tartufata',
                    price: '$45.00'
                },

                {
                    url: 'https://donpeppe.qodeinteractive.com/wp-content/uploads/2019/10/h3-product-img-5a.png',
                    type: 'Francescana',
                    price: '$25.00'
                },

                {
                    url: 'https://donpeppe.qodeinteractive.com/wp-content/uploads/2019/10/h3-product-img-6a.png',
                    type: 'Valdostana',
                    price: '$55.00'
                },
            ]
        }
    }

}
</script>

<style lang='scss' scoped>

    div#pizza-menu-slider{
        height: 55vh;

        div.pizza-card{
            width: 250px;
            height: 55vh;
            background-color: rgb(38, 0, 255);

            div.pizza-object{
                height: 100%;

                div.pizza-immage{
                    height: 60%;
                }

                div.pizza-description{
                    height: 40%;

                    a{
                        color: #B68A2C;
                    }
                }
            }

            div.pizza-btns{
                width: 250px;
                bottom: 0;
                
                button.function-btn{
                    width: 50%;

                    span{
                        font-size: .8rem;
                    }
                }
            }
        }
    }

</style>