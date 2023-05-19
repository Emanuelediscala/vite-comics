<script>
//Definiamo il nome del componente ed eventualmente i componenti che usa (nessuno)
export default {
    name: "AppFooter"
}
</script>

<template>
    <footer>
        <div class="container  d-flex">
            <div class="row col-6 py-5">
                <div class="col-4">
                    <h4>DC COMICS</h4>
                    <ul>
                        <li>Characthers</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>GAMES</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <div>
                        <h4>Shop</h4>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>
                </div>
                <div class="col-4">
                    <h4>DC</h4>
                    <ul>
                        <li>Terms of Use</li>
                        <li>Privacy policy(New)</li>
                        <li>Ad Choises</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </div>
                <div class="col-4">
                    <h4>Sites</h4>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
            </div>
            <div class="col-6 relative" >
                <img src="/public/dc-logo-bg.png"  alt="">
            </div>
        </div>
    </footer>
</template>

<style scoped>
footer {
    background-image: url("/public/footer-bg.jpg");
    background-size: cover;
    height: 450px;
}

h4 {
    color: white;

}

li {
    color: gray;
    list-style-type: none;
    margin: 3px 0;
}

ul {
    padding: 0;
    margin-top: 20px;
}
.relative {
    position: relative;
}
img {
    position: absolute;
    top: -55px;
}

</style>