<template>
    <nav class="container">
        <section class="row py-2">
            <div class="nav-left col-5 d-flex align-items-center justify-content-between">
                <div class="button">
                    <button class="btn btn-danger rounded-0 px-4">Warning</button>
                </div>

                <div class="list">
                    <ul class="d-flex align-items-center mb-0 p-0">
                        <li>
                            <a class="text-decoration-none text-uppercase text-white" href="#">
                                <img class="header-svg" src="@/assets/svg/svg-0.svg" alt="">
                                <span>home</span>
                            </a>
                        </li>

                        <li>
                            <a class="text-decoration-none text-uppercase text-white" href="#">
                                <span>home</span>
                            </a>
                        </li>

                        <li>
                            <a class="text-decoration-none text-uppercase text-white" href="#">
                                <span>home</span>
                            </a>
                        </li>
                    </ul>
                </div>
            </div>

            <!--//! parte al centro -->
            <div class="nav-logo col-2 d-flex align-items-center justify-content-center">
                <img src="@/assets/img/h5-logo-divided-header.png" alt="">
            </div>

            <div class="nav-right col-5 d-flex align-items-center justify-content-between">
                <div class="list">
                    <ul class="d-flex align-items-center mb-0 p-0">
                        <li>
                            <a class="text-decoration-none text-uppercase text-white" href="#">
                                <span>home</span>
                            </a>
                        </li>

                        <li>
                            <a class="text-decoration-none text-uppercase text-white" href="#">
                                <span>home</span>
                            </a>
                        </li>

                        <li>
                            <a class="text-decoration-none text-uppercase text-white" href="#">
                                <span>home</span>
                            </a>
                        </li>
                    </ul>
                </div>

                
                <div class="list">
                    <ul class="d-flex align-items-center mb-0 p-0">
                        <li>
                            <a class="text-decoration-none text-uppercase text-white" href="#">
                                <img class="header-svg" src="@/assets/svg/svg-1.svg" alt="">
                                <span>home</span>
                            </a>
                        </li>

                        <li>
                            <a class="text-decoration-none text-uppercase text-white" href="#">
                                <span>home</span>
                            </a>
                        </li>
                    </ul>
                </div>
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
    
    nav{
        height: 15vh;
        width: 1300px;
        min-width: 960px ;
        position: fixed;
        left: 50%;
        transform: translate(-50%);
        z-index: 2;
        background-color: rgb(16, 94, 68);

        section.row{
            height: 100%;

            button{
                font-size: .7rem;
                text-transform: uppercase;
            }

            img{
                width: 130px;
            }

            div.list{
                height: 100%;

                ul{
                height: 100%;

                    li{
                    list-style-type: none;
                    font-size: .7rem;
                    padding: 0 1.2rem;

                        img.header-svg{
                            width: 23px;
                            fill: #FFFFFF ;
                        }
                    }
                }

            }

        }

        }

        // img{
            //         width: 110px;
            //         vertical-align: middle;
            //         cursor: pointer;
            //     }

</style>