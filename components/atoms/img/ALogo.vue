<template>
    <div class="flex items-center">
        <img :src="src" alt="">
    </div>
</template>

<script>
    export default {
        name: 'ALogo',
        props: {
            src: {
                type: String
            },
        },
    }
</script>

<style scoped>

</style>