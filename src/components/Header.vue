<template>
    <header class="container-fluid">
        <HeaderNav/>
        <HeaderJumbo/>
    </header>
</template>

<script>
import HeaderNav from './HeaderComponents/HeaderNav.vue';
import HeaderJumbo from './HeaderComponents/HeaderJumbo.vue'; 

export default {
    name: 'IndexHeader',
    components : {
        HeaderNav,
        HeaderJumbo
    }

}
</script>

<style lang='scss'>
    
    header{
        min-width: 960px;
        position: relative;
        background-image: url('https://donpeppe.qodeinteractive.com/wp-content/uploads/2019/10/footer-img-2.jpg');
    }

</style>