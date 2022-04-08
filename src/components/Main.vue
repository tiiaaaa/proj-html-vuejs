<template>
    <main>
        <MainFirstSection/>
        <MainSecondSection/>
    </main>
</template>

<script>
import MainFirstSection from './MainComponents/MainFirstSection.vue';
import MainSecondSection from './MainComponents/MainSecondSection.vue';

export default {
    name: 'IndexMain',
    components: {
        MainFirstSection,
        MainSecondSection
    }

}
</script>

<style lang='scss'>


</style>