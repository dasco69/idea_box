<template>
    <div class="inline-flex grid grid-flow-col grid-cols-2">
        <div class="h-full flex items-start justify-evenly flex-col">
            <h1 class="text-white font-concert-one font-light text-9xl mt-20">
                Déposer <br/>
                vos idées
            </h1>
            <div class="w-2/3">
                <p class="text-white">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sapiente earum voluptatibus facere itaque quidem harum. Rem consequuntur animi ex voluptas quasi adipisci quidem. Libero, pariatur. Ipsa quod eum nemo nihil.</p>
            </div>
        </div>
        <div>
            <img :src="require('~/assets/box.png')" alt="">
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