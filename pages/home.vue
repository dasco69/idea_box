<template>
    <div class="inline-flex grid grid-flow-col grid-cols-2 md:grid-cols-1 md:grid-rows-2 md:items-center">
        <div class="h-full flex items-start justify-evenly flex-col md:items-center">
            <h1 class="text-white font-concert-one font-light text-9xl mt-20 md:text-center">
                Déposer <br/>
                vos idées
            </h1>
            <div class="w-2/3 md:text-center">
                <p class="text-white">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sapiente earum voluptatibus facere itaque quidem harum. Rem consequuntur animi ex voluptas quasi adipisci quidem. Libero, pariatur. Ipsa quod eum nemo nihil.</p>
            </div>
        </div>
        <div class="md:flex md:justify-center">
            <img :src="require('~/assets/box.png')" alt="box with rocket" class="md:w-2/5">
        </div>

    </div>
</template>

<script>
    export default {
        name: 'home',
        layout: 'default',
    }
</script>

<style>

</style>