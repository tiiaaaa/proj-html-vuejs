<template>
    <div id="footer-contact" class="col-12 col-lg-6">
        <div class="footer-wrapper d-flex">
            <div class="column px-3">
                <div class="title">
                    <h4 class="text-uppercase mb-4">find your resturants</h4>
                </div>

                <div class="address">
                    <p class="mb-4" v-for="(element, index) in addressList" :key="index">
                        <a class="text-decoration-none" href="#">{{element.street}}</a><br>
                        <a class="text-decoration-none" href="#">{{element.city}}</a><br>
                        <a class="text-decoration-none" href="#">{{element.telephone}}</a><br>
                    </p>
                </div>
            </div>
            <div class="column px-3">vvvs</div>
            <div class="column px-3">wvvw</div>
        </div>
    </div>
</template>

<script>
export default {
    name:'FooterContact',
    data: function(){
        return{
            addressList: [
                {
                    street:'1614 E. Bell Rd #104.',
                    city:'Salerno, AZ 85022',
                    telephone:'(602) 867-1010',
                },

                {
                    street:'204 E. Pizzetta Tommaso.',
                    city:'Sorrento, AZ 85022',
                    telephone:'(358) 867-1010',
                },

                {
                    street:'Vale Puglia 54.',
                    city:'Torre Del Greco AZ 85022',
                    telephone:'(359) 867-1010',
                },

                {
                    street:'Corso Itali AA',
                    city:'Naples, AZ 85022',
                    telephone:'(989) 867-1010',
                },
            ]
        }
    }

}
</script>

<style lang='scss' scoped>
        
    div#footer-contact{
        padding: 6rem 2rem;

        div.column{
            width:calc(100% / 3);

            h4{
                color: #B68A2C;
            }

            p{

                a{
                    letter-spacing: .1rem;
                    color: #858585;
                }
            }
        }
    }
</style>