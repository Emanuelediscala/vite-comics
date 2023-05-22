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
    <section class=" bg-black w-100">
        <div id="jumbo">
            <a href=""></a>
        </div>
        <div class="container d-flex flex-wrap p-5">
            <div v-for="card in cardsList" class="widx6">
                <img :src="card.thumb" alt="">
                <p>{{ card.series }}</p>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
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
    width: 75%;
    height: 150px; 

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
</style>
