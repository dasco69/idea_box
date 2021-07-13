<template>
    <div class="inline-flex w-full md:fixed md:bottom-0 md:left-0 md:justify-center ">
        <ALogo :src="require('~/assets/idea_box.png')" class="md:hidden"/>
        <ul class="inline-flex items-center m-8">
            <li class="ml-6" v-for="item in items" :key="item.id">
                 <div class="flex flex-col items-center">
                     <NuxtLink @click.native='detechItems' class="flex flex-col items-center text-white font-concert-one text-xl" :to="item.path">{{ item.title }}</NuxtLink>
                 </div>
            </li>
        </ul>
    </div>
</template>

<script>
import ALogo from './atoms/img/ALogo.vue'
    export default {
  components: { ALogo },
        name: 'Navbar',
        data() {
            return {
                items: [
                    {
                        title: 'Accueil',
                        path: '/home'
                    },
                    {
                        title: 'Devola',
                        path: '/devola',
                    },
                    {
                        title: 'Good Job',
                        path: '/goodjob',
                    },
                    {
                        title: 'Leads',
                        path: '/leads',
                    }
                ]
            }
        },
        methods: {
            detechItems(element) {
                const path = element.target.href.split('/')[3]
                const pathRoute = this.$route.path.split('/')[1]
                const ancreActive = document.querySelectorAll('.nuxt-link-exact-active .nuxt-link-active')
                document.body.className = ''
                console.log(path)
                switch (path) {
                    case 'home':
                        document.body.classList.add('bg-red-400')
                        break
                    case 'devola':
                        document.body.classList.add('bg-yellow-200')
                        //element.target.style.color = "red"
                        console.log(ancreActive)
                        break
                    case 'goodjob':
                        document.body.classList.add('bg-blue-400')
                        break
                    case 'leads':
                        document.body.classList.add('bg-green-400')
                        break
                    
                    default:
                        document.body.classList.add('bg-red-400')
                        break
                }
            }
        },
    }
</script>

<style scoped>
.nuxt-link-exact-active ,.nuxt-link-active {
    color: #00C3FF;
}
.nuxt-link-exact-active::after, .nuxt-link-active::after {
    content: '';
    background: #00C3FF;
    width: .5rem;
    padding: .5rem;
    border-radius: 50%;
}
</style>