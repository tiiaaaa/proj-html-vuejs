<template>
    <div id="footer-contact" class="col-12 col-lg-6">
        <div class="column-wrapper row d-flex">
            <!-- Prima colonna con link agli indirizzi -->
            <div class="column col-4 px-3">
                <div class="title">
                    <h4 class="text-uppercase fs-5 mb-4">find your resturants</h4>
                </div>

                <div class="address">
                    <p class="mb-4" v-for="(element, index) in addressList" :key="index">
                        <a class="text-decoration-none" href="#">{{element.street}}</a><br>
                        <a class="text-decoration-none" href="#">{{element.city}}</a><br>
                        <a class="text-decoration-none" href="#">{{element.telephone}}</a><br>
                    </p>
                </div>
            </div>
            <!-- Seconda Colonna con orari din apertura/chiusura -->
            <div class="column col-4 px-3">
                <!-- Parte con giornin della settimana e orari -->
                <div class="time-tables">
                    <div class="title">
                        <h4 class="text-uppercase fs-5 mb-4">workin hours</h4>
                    </div>

                    <div class="hours">
                        <h6 class="text-uppercase m-0">monday</h6>
                        <span class="text-danger text-capitalize d-block mb-4">kitchen closed</span>

                        <h6 class="text-uppercase m-0">thusday until friday</h6>
                        <p class="mb-4">9:00 - 22:00</p>

                        <h6 class="text-uppercase m-0">saturday</h6>
                        <p class="mb-4">Saturday at 11a.m. to midnight</p>

                        <h6 class="text-uppercase m-0">Sunday</h6>
                        <p class="mb-4">9:00 - 22:00</p>
                    </div>
                </div>
                
                <!-- Parte bassa con contatti social -->
                <div class="social d-flex">
                    <div>
                        <h6 class="text-uppercase m-0">follow us:</h6>
                    </div>

                    <a class="text-decoration-none" href="https://twitter.com/QodeInteractive">
                        <span class="social-twitter"></span>
                    </a>
                </div>
            </div>
            <!-- Terza Colonna -->
            <div class="column col-4 px-3">
                <div>
                    <h3 class="text-uppercase text-white lh-sm">
                        The Don Peppe crew first and foremost values an authentic, well baked slice of pizza.
                    </h3>
                </div>
            </div>
        </div>

        <div class="row-wrapper row">
            <div class="col-6 d-flex align-items-end">
                <p class="fw-light">
                    <span class="date me-1">2020</span>
                    <span class="text">Quode Interactive</span>
                </p>
            </div>
            <div class="col-6 text-end">
                <img src="https://donpeppe.qodeinteractive.com/wp-content/uploads/2019/10/footer-bottom-img.png" alt="">
            </div>
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
            ],
        }
    }

}
</script>

<style lang='scss' scoped>
        
    div#footer-contact{
        padding: 6rem 3rem 2rem 3rem;

        div.column-wrapper{

            div.column{

                h4, h6{
                    color: #B68A2C;
                }

                p{
                    font-size: .9rem;
                    color: #858585;

                    a{
                        letter-spacing: .1rem;
                        color: #858585;
                    }
                }

                div.social{

                    a{
                        color: #fff;
                        
                        span.social-twitter::before{
                            content: '' ;

                        }
                    }
                }
            }
        }

        div.row-wrapper{

            p{

                font-size: .8rem;
                letter-spacing: .1rem;

                span.date{
                    color: #B68A2C;
                }

                span.text{
                    color: #339966;
                }
            }
        }
    }
</style>