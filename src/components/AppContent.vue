<script>
import { stringifyExpression } from '@vue/compiler-core';


//Definiamo il nome del componente ed eventualmente i componenti che usa (nessuno)
export default {
    name: "AppContent",
    props: {
        cardsList: Object
    }
}

</script>
<template>
    <section class=" bg-black w-100 relative">
        <div id="jumbo">
        </div>
        <button class="btn btn-primary btnabsolute">CURRENT SERIES</button>
        <div class="container d-flex flex-wrap justify-content-center relative p-5">
            <div v-for="card in cardsList" class="widx6 p-2">
                <img :src="card.thumb"  alt="">
                <p>{{ card.series }}</p>
            </div>
            <button class="btn btn-primary">LOAD MORE</button>
        </div>
        
    </section>
</template>

<style scoped >
div#jumbo {
    background-image: url(../../public/jumbotron.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    height: 400px;
}
.widx6 {
    width: calc(100% / 6);
}
img {
    width: 100%;
    height: 200px;
    object-fit: cover;
    object-position: top ;
}
button {
    width: 300px;
}
.btnabsolute {
    position:absolute;
    bottom:61%;
    left: 400px;
}

p {
    font-weight: 600;
    color: white;
    text-align: center;
}
a {
    color: white;
    font-size: 24px;
}
.relative {
    position: relative;
}
</style>
