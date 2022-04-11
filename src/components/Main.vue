<template>
    <main class="container-fluid">
        <MainFirstSection/>
        <MainSecondSection/>
        <MainThirdSection/>
        <MainFourthSection/>
        <MainFifthSection/>
    </main>
</template>

<script>
import MainFirstSection from './MainComponents/MainFirstSection.vue';
import MainSecondSection from './MainComponents/MainSecondSection.vue';
import MainThirdSection from './MainComponents/MainThirdSection.vue';
import MainFourthSection from './MainComponents/MainFourthSection.vue';
import MainFifthSection from './MainComponents/MainFifthSection.vue'; 

export default {
    name: 'IndexMain',
    components: {
        MainFirstSection,
        MainSecondSection,
        MainThirdSection,
        MainFourthSection,
        MainFifthSection,
    }

}
</script>

<style lang='scss'>


</style>