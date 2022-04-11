<template>
    <section id='pizza-deals' class="row">
        <!-- Colonna Sinistra -->
        <div id="deals-places" class="col-12 col-md-6">
            <!-- Div che raggruppa le varie voci -->
            <div class="deals-wrapper text-white">
                <!-- Prima scritta in alto -->
                <div id="title" class="pb-4">
                    <span class="text-danger text-uppercase d-block mb-3">made whit love</span>
                    <h1 class="text-uppercase m-0">delish pizza deals</h1>
                </div>
                <!-- Secondo Div che wrappa due div per metterli a finaco -->
                <div class="event d-flex text-center py-4" v-for="(event, index) in EventLIst" :key="index">

                    <!-- Div con data e mese -->
                    <div class="date">
                        <h1 class="fw-bold m-0">{{event.date}}</h1>
                        <p class="text-uppercase fw-bold m-0">{{event.month}}</p>
                    </div>
                    <!-- Div con il testo dell evento -->
                    <div class="date-text ps-5">
                        <h4 class="mb-4">
                            <a class="text-decoration-none text-white text-uppercase" href="#">
                                {{event.event}}
                            </a>
                        </h4>

                        <p class="text-capitalize m-0">{{event.location}}</p>
                    </div>
                </div>
                <div></div>
                <div></div>
            </div>
        </div>

        <!-- Colonna Destra -->
        <div id="deals-immage" class="col-12 col-md-6 p-0">
            <img class="img-fluid" src="@/assets/img/h3-img-5a.jpg" alt="">
        </div>

    </section>
</template>

<script>
export default {
    name:'PizzaDeals',

    data: function(){
        return{

            EventLIst: [

                {
                    date:'02',
                    month:'nov',
                    event:'Traditional Neapolitan Pies In Kyoto Pizza Mercato',
                    location:'204 e. pizzetta tommaso'
                },

                {
                    date:'03',
                    month:'nov',
                    event:'terarazza patio dining space opening this weekend',
                    location:'204 c. pizzetta giuseppe'
                },

                {
                    date:'05',
                    month:'nov',
                    event:'Traditional Neapolitan Pies In Kyoto Pizza Mercato',
                    location:'204 b. pizzetta maria'
                },
            ]
        }
    }

}
</script>

<style lang='scss' scoped>
    section#pizza-deals{

        div#deals-places{
            padding: 4rem 6rem;
            background-color: #1c1c1c;

            div.deals-wrapper{
                
                div#title{

                    span{
                    font-size: .8rem;
                    font-weight: 600;
                    letter-spacing: .2rem;
                    }
                }

                div.event{

                    border-bottom: dotted;
                    border-color: #ffa323;

                    div.date{

                    h1{
                        font-size: 3.8rem;
                        color: #ab4027;
                    }

                    p{
                        font-size: 1.8rem;
                    }
                }

                div.date-text{
                    text-align: start;

                    h4{
                        font-size: 1.5rem;
                        line-height: 2.2rem;
                        letter-spacing: .1rem;
                    }

                    p{
                        font-size: .8rem;
                        color: #ab4027;
                    }
                }

                }
                
            }
        }

        div#deals-immage{
            
            img{
                height: 100%;
                object-fit: cover;
            }
        }
    }

</style>