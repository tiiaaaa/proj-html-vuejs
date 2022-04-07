<template>
    <nav class="container">
        <section class="row align-items-center text-white py-3">
            <div class="col-3">
                <button type="button" class="btn btn-danger">Danger</button>
            </div>

            <div class="col-6">
                <div>
                    <ul class="d-flex justify-content-evenly mb-0 p-0">
                        <li class="d-flex align-items-center">
                            <a class="text-uppercase text-white text-decoration-none" href="#">
                                home
                            </a>
                        </li>

                        <li class="d-flex align-items-center">
                            <a class="text-uppercase text-white text-decoration-none" href="#">
                                home
                            </a>
                        </li>

                        <li class="d-flex align-items-center">
                            <a class="text-uppercase text-white text-decoration-none" href="#">
                                home
                            </a>
                        </li>

                        <li class="d-flex align-items-center">
                            <img src="@/assets/img/h5-logo-divided-header.png" alt="">
                        </li>

                        <li class="d-flex align-items-center">
                            <a class="text-uppercase text-white text-decoration-none" href="#">
                                home
                            </a>
                        </li>
                        <li class="d-flex align-items-center">
                            <a class="text-uppercase text-white text-decoration-none" href="#">
                                home
                            </a>
                        </li>
                        <li class="d-flex align-items-center">
                            <a class="text-uppercase text-white text-decoration-none" href="#">
                                home
                            </a>
                        </li>
                    </ul>
                </div>
            </div>

            <div class="col-3">
                <ul class="d-flex justify-content-evenly mb-0 p-0">
                    <li class="d-flex align-items-center">
                        <a class="text-uppercase text-white text-decoration-none" href="#">
                            home
                        </a>
                    </li>
                    <li class="d-flex align-items-center">
                        <a class="text-uppercase text-white text-decoration-none" href="#">
                            home
                        </a>
                    </li>
                </ul>
            </div>
        </section>
    </nav>
</template>

<script>
export default {
    name: 'HeaderNav'

}
</script>

<style lang='scss' scoped>
    
    nav.container{
        // height: 15vh;

        section.row{
            // height: 100%;

            li{
            list-style-type: none;

                a{
                    font-size: .8rem
                }

                img{
                    width: 110px;
                    vertical-align: middle;
                    cursor: pointer;
                }
            }
        }
    }

</style>