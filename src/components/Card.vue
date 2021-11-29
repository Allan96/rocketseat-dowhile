<template>
<div class="card" :class="product.list ? 'list' : ''">
    <div class="box-left">
        <Tag :text="product.labelTag" :icon="product.iconTag" />

        <CardImage />
    </div>
    <div class="box-right">
        <span class="c-nmedium medium block text-right" v-show="product.brand">{{ product.brand }}</span>

        <span class="c-ndark large block" v-show="product.name">{{ product.name }}</span>

        <span class="c-smedium medium block text-right" v-show="product.priceWithDiscount">{{ product.priceWithDiscount }}</span>

        <span class="c-ndark large block text-right" v-show="product.price">{{ product.price }}</span>

        <Button v-if="product.labelButton"> {{product.labelButton}} </Button>
    </div>
</div>
</template>

<script>
import CardImage from '@/components/CardImage'
import Button from '@/components/Button'
import Tag from '@/components/Tag'
export default {
    props: {
        product: {
            type: Object,
            default: null
        }
    },
    components: {
        Tag,
        CardImage,
        Button
    },
}
</script>

<style>

</style>
