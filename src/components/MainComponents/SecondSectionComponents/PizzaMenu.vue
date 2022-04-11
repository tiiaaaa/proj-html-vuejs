<template>
    <div id="pizza-menu" class="col-12 col-lg-6 d-flex align-items-center justify-content-center p-5">
        <div id="pizza-menu-list d-flex flex-column">
            <div class="pizza-menu-voice">
                <h2 class="text-uppercase">specials*</h2>
                <span>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Modi et consequuntur possimus veritatis! Fuga animi, repellat vel quae omnis sed illo cum maiores laborum aperiam consequuntur cumque maxime expedita consequatur.</span>
            </div>
            <div class="pizza-menu-voice"></div>
            <div class="pizza-menu-voice"></div>
            <div class="pizza-menu-voice"></div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'PizzaMenu',
}
</script>

<style lang='scss' scoped>

    div#pizza-menu-list{
        
        div.pizza-menu-voice{
            
            span{
            color: #b2b2b2;

            }
        }
    }


</style>