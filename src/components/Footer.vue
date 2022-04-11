<template>
    <footer>
        <section class="rowc py-3">
            <FooterContact/>
            <FooterImmage/>
        </section>
    </footer>
</template>

<script>
import FooterContact from './FooterComponents/FooterContact.vue';
import FooterImmage from './FooterComponents/FooterImmage.vue';

export default {
    name: 'IndexFooter',
    components: {
        FooterContact,
        FooterImmage,
    }

}
</script>

<style lang='scss'>

    footer{

        div#footer-contact,
        div#footer-immage{
            height: 80vh;
            background-color: #1b1b1b;
        }
    }


</style>