<template>
<button v-if="$slots.default">
    <slot> </slot>
</button>
</template>

<script>
export default {
    props: {
    }
}
</script>

<style lang="scss" scoped>
button {
    border: 0;
}
</style>
