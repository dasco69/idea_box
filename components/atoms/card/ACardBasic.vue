<template>
    <div class="bg-white rounded-2xl w-3/4 p-20 md:p-10 md:w-10/12">
        <div>
            <slot name="title"></slot>
        </div>
        <div class="mt-10 mb-10">
            <slot name="input"></slot>
        </div>
        <div>
            <slot name="button"></slot>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'ACardBasic'
    }
</script>

<style scoped>

</style>