<template>
    <div id="main-first-section">
        <MiniCard/>
        <PizzaSlider/>
    </div>
</template>

<script>
import MiniCard from './FirstSectionComponents/MiniCard.vue';
import PizzaSlider from './FirstSectionComponents/PizzaSlider.vue';

export default {
    name: 'MainFirstSection',
    components:{
        MiniCard,
        PizzaSlider
    }

}
</script>

<style lang='scss' scoped>
    
</style>