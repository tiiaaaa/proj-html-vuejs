<template>
    <div id="main-fourth-section" class="pb-5">
        <PizzaBrandList/>
        <TheBeastPizza/>
        <SliderPizzaImmages/>
    </div>
</template>

<script>
import PizzaBrandList from './FourthSectionComponents/PizzaBrandList.vue';
import TheBeastPizza from './FourthSectionComponents/TheBeastPizza.vue';
import SliderPizzaImmages from './FourthSectionComponents/SliderPizzaImmages.vue';

export default {
    name:'MainFourthsection',
    components:{
        PizzaBrandList,
        TheBeastPizza,
        SliderPizzaImmages,
    }

}
</script>

<style lang='scss' scoped>

</style>