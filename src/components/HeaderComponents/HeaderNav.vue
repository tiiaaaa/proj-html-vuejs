<template>
    <div id="nav-bar">
        <nav class="container">
            <section class="row py-2">
                <div class="nav-left col-5 d-flex align-items-center justify-content-between">
                    <div class="button">
                        <button class="btn btn-danger rounded-0 px-4">order online</button>
                    </div>
                    
                    <!-- Lista Sinistra -->
                    <div class="list">
                        <ul class="d-flex align-items-center mb-0 p-0">
                            <li v-for="(element, index) in navFirstList" :key="index">
                                <img class="header-svg" :src="element.svg" alt="">
                                <a class="text-decoration-none text-uppercase text-white" href="#">
                                    <span>{{element.link}}</span>
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>

                <!--// Logo centrale -->
                <div class="nav-logo col-2 d-flex align-items-center justify-content-center">
                    <img src="@/assets/img/h5-logo-divided-header.png" alt="">
                </div>
                
                <!-- Prima Lista a destra -->
                <div class="nav-right col-5 d-flex align-items-center justify-content-between">
                    <div class="list">
                        <ul class="d-flex align-items-center mb-0 p-0">
                            <li v-for="(element, index) in navSecondList" :key="index">
                                <a class="text-decoration-none text-uppercase text-white" href="#">
                                    <span>{{element.link}}</span>
                                </a>
                            </li>
                        </ul>
                    </div>

                    <!-- Seconda Lista a Destra -->
                    <div class="list">
                        <ul class="d-flex align-items-center mb-0 p-0">
                            <li v-for="(element, index) in navThirdList" :key="index">
                                <a class="text-decoration-none text-uppercase text-white" href="#">
                                    <img class="header-svg" :src="element.svg" alt="">
                                    <span>{{element.link}}</span>
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </section>
        </nav>
    </div>
</template>

<script>
export default {
    name: 'HeaderNav',
    data: function(){
        return{
            navFirstList: [
                {
                    svg: require('@/assets/svg/svg-0.svg'),
                    link: 'home'
                },

                {
                    link: 'pages'
                },

                {
                    link: 'menu'
                },
            ],

            navSecondList: [

                {
                    link: 'events'
                },

                {
                    link: 'blog'
                },

                {
                    link: 'landing'
                },
            ],

            navThirdList: [

                {
                    svg: require('@/assets/svg/svg-1.svg'),
                    link: 'cart'
                },

                {
                    svg: require('@/assets/svg/svg-0.svg'),
                    link: 'search'
                }
            ]
        }
    }

}
</script>

<style lang='scss' scoped>

    div#nav-bar{
        height: 15vh;
        width: 100%;
        position: fixed;
        left: 50%;
        transform: translate(-50%);
        z-index: 2;
        background-color: #1b1b1b;

        nav{
        width: 100%;
        min-width: 960px ;

        section.row{
            height: 100%;

            button{
                font-size: .8rem;
                text-transform: uppercase;
            }

            img{
                width: 140px;
            }

            div.list{
                height: 100%;

                ul{
                height: 100%;

                    li{
                    list-style-type: none;
                    font-size: .8rem;
                    padding: 0 1.2rem;

                        img.header-svg{
                            width: 23px;
                            fill: #FFF;
                            color: #FFF ;
                        }
                    }
                }

            }

        }

    }
    }

</style>