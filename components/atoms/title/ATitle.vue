<template>
    <div>
        <h1 class="font-concert-one text-5xl " :class="classCss">
            {{ title }}
        </h1>
    </div>
</template>

<script>
    export default {
        name: 'ATitle',
        props: {
            title: {
                type: String
            },
            classCss: {
                type: String
            },
        },
    }
</script>

<style scoped>

</style>