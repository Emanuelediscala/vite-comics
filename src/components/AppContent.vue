<script>
import { stringifyExpression } from '@vue/compiler-core';


//Definiamo il nome del componente ed eventualmente i componenti che usa (nessuno)
export default {
    name: "AppContent",
    props: {
        card: [
            {
                thumb: String,
                price: String,
                series: String,
                type: String
            }
        ]
    }
}

</script>
<template>
    <section class=" bg-black w-100">
        <div>
            <a href="" class="text"></a>
            <div>
                {{ card }}
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
div {
    background-image: url(../../public/jumbotron.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    height: 500px;
}

a {
    color: white;
    font-size: 24px;
}
</style>
