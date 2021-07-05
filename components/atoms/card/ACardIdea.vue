<template>
    <div class="bg-white rounded-2xl w-full h-body p-20">
        <div>
            <slot name="title"></slot>
        </div>
        <div class="mt-5 mb-10">
            <slot name="point"></slot>
        </div>
        <div>
            <slot name="list"></slot>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'ACardIdea'
    }
</script>

<style scoped>

</style>