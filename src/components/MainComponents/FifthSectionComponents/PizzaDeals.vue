<template>
    <section id='pizza-deals' class="row">
        <!-- Colonna Sinistra -->
        <div id="deals-places" class="col-12 col-sm-6 p-5">
            <div class="deals-wrapper">
                

            </div>
        </div>

        <!-- Colonna Destra -->
        <div id="deals-immage" class="col-12 col-sm-6 p-0">
            <img class="img-fluid" src="@/assets/img/h3-img-5a.jpg" alt="">
        </div>

    </section>
</template>

<script>
export default {
    name:'PizzaDeals'

}
</script>

<style lang='scss' scoped>
    section#pizza-deals{
        height: 70vh;

        div#deals-immage{
            
            img{
                height: 100%;
                object-fit: cover;
            }
        }
    }

</style>