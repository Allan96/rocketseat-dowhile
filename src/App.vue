<template>
<div id="app">
    
    <Card :product="items" />


</div>
</template>

<script>
import Card from '@/components/Card'
export default {
    name: 'App',
    components: {
        Card
    },
    data() {
        return {
            items: {
                brand: "Adidas",
                name: "ZX 5000 Vieux Lyon",
                price: "899,99",
                priceWithDiscount: "699,99",
                labelButton: "Comprar",
                labelTag: "Black Friday",
                iconTag: true,
                list: true
            }
        }
    }
}
</script>

<style lang="scss">
</style>
