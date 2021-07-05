<template>
    <div>
        <ul class="inline-flex m-8">
            <li class="ml-6" v-for="item in items" :key="item.id">
                 <div class="flex flex-col items-center">
                     <NuxtLink @click.native='detechItems' class="flex flex-col items-center" :to="item.path">{{ item.title }}</NuxtLink>
                 </div>
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
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
                document.body.className = ''

                switch (path) {
                    case 'home':
                        console.log('home')
                        document.body.classList.add('bg-red-400')
                        break;
                    case 'devola':
                        console.log('devola')
                        document.body.classList.add('bg-yellow-200')
                        break
                    case 'goodjob':
                        console.log('goodjob')
                        document.body.classList.add('bg-blue-400')
                        break
                    case 'leads':
                        console.log('leads')
                        document.body.classList.add('bg-green-400')
                        break
                    
                    default:

                        break;
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