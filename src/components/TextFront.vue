<script>
export default {
    props: {
        text: { type: String, required: true },
    },
    components: { Card }
};
import Card from '../components/Card.vue';
</script>
<template>
    <main class="main pt-5 pb-5 text-center justify-contents-center px-3 px-md-5">
        <div class="row align-items-center">
            <h1 class="mb-5 mb-lg-4 col-lg-6" style="color:#464646;" v-html="text"></h1>
            <div class="col-lg-6">
                <Card content="Sou bom em usar <strong>Vue.js + Nuxt.js</strong> para iniciar um projeto <strong>:)</strong>" />
                <Card content="Vamos construir um <strong>novo projeto</strong> juntos!" />  
            </div>
            
        </div>
    </main>
</template>
<style scoped>
h1 {
    font-weight: 300;
}
</style>
