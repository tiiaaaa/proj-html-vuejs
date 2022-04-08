<template>
    <nav class="container">
        <section class="row align-items-center text-white text-center py-3">
            <!-- Bottone Rosso sulla sinistra -->
            <div class="col-3">
                <button type="button" class="btn-danger rounded-0 btn-sm py-1 px-4 text-uppercase">order online</button>
            </div>
            
            <!-- Lista di link centrale con img-logo -->
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
            
            <!-- Link sulla destra  -->
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
    name: 'HeaderNav',
    data: function(){
        return{
            navList: [
                {
                    svg: '@/assets/svg/svg-0.svg',
                    link: 'home'
                },

                {
                    link: 'pages'
                },

                {
                    link: 'menu'
                },

                {
                    link: 'events'
                },

                {
                    link: 'blog'
                },

                {
                    link: 'landing'
                },
            ]
        }
    }

}
</script>

<style lang='scss' scoped>
    
    nav.container{
        height: 15vh;
        min-width: 960px;
        position: sticky;
        top: 0;
        z-index: 2;

        section.row{
            // height: 100%;

            button{
                font-size: .7rem;
            }

            li{
            list-style-type: none;

                a{
                    font-size: .7rem
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