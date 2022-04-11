<template>
    <div id="footer-contact" class="col-12 col-md-6">
        <div class="footer-wrapper d-flex">
            <div class="column px-3">
                <div class="title">
                    <h4 class="text-uppercase">find your resturants</h4>
                </div>

                <div class="address">
                    <p>
                        <a class="text-decoration-none" href="#">
                            1614 E. Bell Rd #104.<br>
                            Salerno, AZ 85022<br>
                            (602) 867-1010
                        </a>
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