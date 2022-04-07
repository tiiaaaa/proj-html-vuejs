<template>
    <header>
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
        background-color: #1b1b1b;
    }

</style>