<script>
//Definiamo il nome del componente ed eventualmente i componenti che usa (nessuno)
export default {
    name: "AppContent",
};
</script>

<template>
    <section class="bg-black w-100">
        <div class="container p-5">
            <a href="" class="text">Content Goes here</a>
        </div>
    </section>
    <section class="bg-primary w-100">
        <div class="container p-5">
            <div>
                <nav>
                    <ul class="nav">
                        <li class="nav-item d-flex align-items-center">
                            <img src="/public/buy-comics-digital-comics.png"  alt="">
                            <a class="nav-link active" aria-current="page" href="#">DIGITAL COMICS</a>
                        </li>
                        <li class="nav-item d-flex align-items-center">
                            <img src="/public/buy-comics-merchandise.png" alt="">
                            <a class="nav-link" href="#">DC MERCHANDISE</a>
                        </li>
                        <li class="nav-item d-flex align-items-center">
                            <img src="/public/buy-comics-subscriptions.png" alt="">
                            <a class="nav-link" href="#">Subscription</a>
                        </li>
                        <li class="nav-item d-flex align-items-center">
                            <img src="/public/buy-comics-shop-locator.png" alt="">
                            <a class="nav-link" href="#">COMIC SHOP LOCATOR</a>
                        </li>
                        <li class="nav-item d-flex align-items-center">
                            <img src="/public/buy-dc-power-visa.svg" alt="">
                            <a class="nav-link" href="#">DC POWER VISA</a>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
    </section>
</template>

<style scoped>
nav img {
    width: 50px;
}
a {
    color: white;
}
</style>
