<template>
  <div class="card-image" :style="`background-image: url('${url}')`">
  </div>
</template>

<script>
export default {
props:{
    url:{
        type: String,
        default: 'https://placekitten.com/g/300/300'
    }
}
}
</script>

<style>

</style>