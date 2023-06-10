<script>
import backBtn from '../components/backBtn.vue';
import Card from '../components/Card.vue';
export default {
    components: { backBtn, Card }
}
</script>
<template>
    <main class="container container-fluid mt-0 justify-content-center">
        <aside>
            <backBtn />
            <div class="mt-3 mb-4 mb-lg-5 text-center">
                <h2>Veja minhas <strong>skills</strong> abaixo.</h2>
            </div>
            <div class="text-center container row mx-0 justify-content-center">
                <Card class="col-12 col-sm-7 col-md-5 col-lg-4" content="<strong>HTML5 / CSS3</strong>" />
                <Card class="col-12 col-sm-7 col-md-4 col-lg-3" content="<strong>Bootstrap 5</strong>" />
                <Card class="col-12 col-sm-5 col-md-3" content="<strong>Figma</strong>" />
                <Card class="col-12 col-sm-5 col-md-3" content="<strong>Node.js</strong>" />
                <Card class="col-12 col-sm-5 col-md-6" content="<strong>Vue.js</strong>" />
                <Card class="col-12 col-sm-5 col-md-4" content="<strong>SCRUM</strong>" />
            </div>
        </aside>
        <div class="mt-3 mb-3 mb-md-4 mb-lg-5 mx-lg-5 text-center">
                <h2>Além disso, tenho grande <strong>disposição</strong> para aprender sobre outras áreas em TI.</h2>
                <RouterLink class="mb-3 mb-md-0 col-6 col-md-4 col-lg-3 mx-3" id="btn-contact" to="/contact">CONTATO</RouterLink>
        </div>
    </main>
</template>
