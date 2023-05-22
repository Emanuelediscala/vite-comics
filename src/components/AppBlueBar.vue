<script>
//Definiamo il nome del componente ed eventualmente i componenti che usa (nessuno)
export default {
    name: "AppBlueBar",
    data(){
        return {
            icons: [
                {
                    name:'DIGITAL COMICS',
                    path:'/public/buy-comics-digital-comics.png'
                },
                {
                    name: 'DC MERCHANDISE',
                    path:'/public/buy-comics-merchandise.png'
                },
                {
                    name:'SUBSCRIPTION',
                    path:'/public/buy-comics-shop-locator.png'
                },
                {
                    name:'COMIC SHOP LOCATOR',
                    path:'/public/buy-comics-subscriptions.png'
                },
                {
                    name:'DC POWER VISA',
                    path:'/public/buy-dc-power-visa.svg'
                }
            ]
    }
}
}
</script>

<template>
        <section class="bg-primary w-100">
            <div class="container p-3">
                <nav class="w-100">
                    <ul class="nav d-flex justify-content-around">
                        <li v-for="el in icons" class="nav-item d-flex align-items-center" >
                            <img :src="el.path" alt="">
                            <a class="nav-link active" aria-current="page" href="#">{{ el.name }}</a>
                        </li>
                    </ul>
                </nav>
            </div>
        </section>
</template>

<style scoped lang="scss">
nav img {
    width: 50px;
}
a {
    color: white;
}
section.bg-primary {
    z-index: 999;
    position: relative;
}
</style>
