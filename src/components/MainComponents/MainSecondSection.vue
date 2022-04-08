<template>
    <div id='second-section'>
        <section class="row py-2">
            <PizzaSpecial/>
            <PizzaMenu/>
        </section>
    </div>
</template>

<script>
import PizzaSpecial from './SecondSectionComponents/PizzaSpecial.vue';
import PizzaMenu from './SecondSectionComponents/PizzaMenu.vue';

export default {
    name: 'MainSecondSection',
    components: {
        PizzaSpecial,
        PizzaMenu
    }

}
</script>

<style lang='scss'>

    div#pizza-special,
    div#pizza-menu{
        height: 70vh;
        background-color: aquamarine;
    }

</style>