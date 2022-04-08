<template>
    <div id="main-third-section">
        <BuildPizzaCollage/>
        <GuysImmages/>
    </div>
</template>

<script>
import BuildPizzaCollage from './ThirdSectionComponents/BuildPizzaCollage.vue';
import GuysImmages from './ThirdSectionComponents/GuysImmages.vue';

export default {
    name: 'MainThirdSection',
    components:{
        BuildPizzaCollage,
        GuysImmages,
    }

}
</script>

<style>

</style>