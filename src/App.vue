<template>
    <div id="app">
        <Header/>
        <Main/>
        <Footer/>
    </div>
</template>

<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
@import './assets/style/style.scss';

#app {
  font-family: 'Oswald', sans-serif;

    // Stilizzazione btn next e prev comune a più components
    div.circle-btn{
              height: 85px;
              width: 85px;
              cursor: pointer;
              background-color: #f7f7f7;

              span{
                  font-size: .8rem;
                  font-weight: 600;
                  letter-spacing: .2rem;
              }
          }

          div.prev-btn{
              top: 50%;
              left: -50px;
              transform: translate(0, -50%);
              transform: rotate(90deg);
          }

          div.next-btn{
              top: 50%;
              right: -50px;
              transform: translate(0, -50%);
              transform: rotate(-90deg);
          }
}
</style>
