<template>
    <div id="pizza-special" class="col-6 position-relative">
        <img class="position-absolute" src="@/assets/img/h1-img-7n.png" alt="">
    </div>
</template>

<script>
export default {
    name: 'PizzaSpecial',

}
</script>

<style lang='scss' scoped>

    div#pizza-special{
        background-image: url('@/assets/img/h1-img-4.jpg');
        background-position: center;
        background-size: cover;
        background-repeat: no-repeat;

        img{
            width: 220px;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
        }
    }
    

</style>