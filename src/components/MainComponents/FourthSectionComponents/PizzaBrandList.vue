<template>
    <section id="pizza-brand-list" class="row">
        <div class="col-12 d-flex align-items-center">
            <ul class="d-flex mb-0">
                <li v-for="(brand, index) in PizzaBrandList" :key="index">
                    <a class="text-decoration-none" href="#">
                        <img :src="require('@/assets/img/' + brand.url)" alt="">
                    </a>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name:'PizzaBrandList',
    data: function(){
        return{

            PizzaBrandList:[

                    {
                        url: 'h1-clients-img-1.png'
                    },

                    {
                        url: 'h1-clients-img-2.png'
                    },

                    {
                        url: 'h1-clients-img-3.png'
                    },

                    {
                        url: 'h1-clients-img-4.png'
                    },

                    {
                        url: 'h1-clients-img-5.png'
                    },
            ]
        }
    }

}
</script>

<style lang='scss' scoped>

    section#pizza-brand-list{
        height: 43vh;
        background-color: #f7f7f2;

        li{
            list-style-type: none;
        }
    }

</style>