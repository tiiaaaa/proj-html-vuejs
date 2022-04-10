<template>
    <main class="container-fluid">
        <MainFirstSection/>
        <MainSecondSection/>
        <MainThirdSection/>
        <MainFourthSection/>
    </main>
</template>

<script>
import MainFirstSection from './MainComponents/MainFirstSection.vue';
import MainSecondSection from './MainComponents/MainSecondSection.vue';
import MainThirdSection from './MainComponents/MainThirdSection.vue';
import MainFourthSection from './MainComponents/MainFourthSection.vue';

export default {
    name: 'IndexMain',
    components: {
        MainFirstSection,
        MainSecondSection,
        MainThirdSection,
        MainFourthSection,
    }

}
</script>

<style lang='scss'>


</style>