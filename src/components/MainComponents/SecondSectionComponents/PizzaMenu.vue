<template>
    <div id="pizza-menu" class="col-12 col-lg-6 p-0">
        <div id="pizza-menu-specials">
            <!-- Blocco del titolo specials -->
            <div class="pizza-menu-title pb-4">
                <h2 class="text-uppercase fs-1 mb-3">specials*</h2>
                <span class="fw-light">Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis libero molestias sunt vel debitis quos non.</span>
            </div>
            <!-- blocco con le varie voci del menu -->
            <div class="pizza-menu-voice pt-3">
                <!-- singola voce -->
                <div class="voice d-flex py-3" v-for="(element, index) in menuList" :key="index">

                    <div class="food-price pe-3">
                        <h4 class="fs-4">{{element.price}}</h4>
                    </div>

                    <div class="food">
                        <h4 class="text-uppercase fs-4">{{element.foodName}}</h4>
                        <span class="fw-light">{{element.description}}</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'PizzaMenu',
    data: function(){
        return{
            
            menuList: [

                {
                    price: '$10',
                    foodName:'combo piccolo',
                    description:'Lorem ipsum dolor sit amet consectetur adipisicing elit.'
                },

                {
                    price: '$20',
                    foodName:'combo mezzo',
                    description:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto, culpa? Exercitationem assumenda'
                },

                {
                    price: '$30',
                    foodName:'combo grande',
                    description:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto,'
                }
            ]
        }
    }
}
</script>

<style lang='scss' scoped>

    div#pizza-menu-specials{
        
        padding: 5rem 8rem;

        span{
                font-size: 1.1rem;
                color: #767676;
            }

        div.pizza-menu-voice{

            div.voice{

                div.food-price{

                    h4{
                        color: #AB4027;
                    }
                }
            }
        }
    }


</style>