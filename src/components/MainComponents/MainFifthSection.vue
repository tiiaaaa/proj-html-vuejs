<template>
    <section id="fifth-section">
        <PizzaDeals/>
        <SelectForPrenotation/>
    </section>
</template>

<script>

import PizzaDeals from './FifthSectionComponents/PizzaDeals.vue';
import SelectForPrenotation from './FifthSectionComponents/SelectForPrenotation.vue';

export default {
    name:'FifthSection',
    components:{
        PizzaDeals,
        SelectForPrenotation,
    }

}
</script>

<style lang='scss' scoped>

</style>