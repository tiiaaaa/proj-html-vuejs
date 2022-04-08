<template>
    <main class="container-fluid">
        <MainFirstSection/>
        <MainSecondSection/>
        <MainThirdSection/>
    </main>
</template>

<script>
import MainFirstSection from './MainComponents/MainFirstSection.vue';
import MainSecondSection from './MainComponents/MainSecondSection.vue';
import MainThirdSection from './MainComponents/MainThirdSection.vue';

export default {
    name: 'IndexMain',
    components: {
        MainFirstSection,
        MainSecondSection,
        MainThirdSection,
    }

}
</script>

<style lang='scss'>


</style>