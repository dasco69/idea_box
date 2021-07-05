<template>
    <div>
        <label for="textaea" class="font-concert-one text-lg" :class="classCss">{{ label }}</label>
        <textarea name="desire" id="desire" cols="30" rows="10" class="bg-gray-50 p-4 rounded-2xl" placeholder="Lâches un mot">
            
        </textarea>
    </div>
</template>

<script>
    export default {
        name:'ATextArea',
        props: {
            label: {
                type: String
            },
            classCss: {
                type: String
            }
        },
    }
</script>

<style scoped>

</style>