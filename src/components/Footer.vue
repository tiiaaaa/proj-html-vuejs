<template>
    <footer>
        <section class="row pt-3">
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
            background-image: url('https://donpeppe.qodeinteractive.com/wp-content/uploads/2019/10/footer-img-2.jpg');
        }
    }


</style>